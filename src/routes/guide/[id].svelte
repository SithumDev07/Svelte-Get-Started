<script context="module">
  export async function load({ fetch, page }) {
    const id = page.params.id;
    const res = await fetch(`https://jsonplaceholder.typicode.com/posts/${id}`);
    const guide = await res.json();

    if (res.ok) {
      return {
        props: {
          guide,
        },
      };
    }

    return {
      status: res.status,
      error: new Error("Could not load the data from the API"),
    };
  }
</script>

<script>
  export let guide;
</script>

<div class="guide">
  <h1>{guide.title}</h1>
  <p>{guide.body}</p>
</div>

<style>
  .guide {
    max-width: 960px;
    margin: 4rem auto;
    font-family: "Montserrat", sans-serif;
    font-size: 3vw;
    color: blue;
    border: 1px dotted #0000ff;
    padding: 3rem;
  }
  p {
    margin-top: 2rem;
  }
</style>
