<script context="module">
  export async function load({ fetch }) {
    const res = await fetch("https://jsonplaceholder.typicode.com/posts");
    const guides = await res.json();

    if (res.ok) {
      return {
        props: {
          guides,
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
  export let guides;
</script>

<div class="guides">
  <ul>
    {#each guides as guide}
      <li><a href={`/guide/${guide.id}`}>{guide.title}</a></li>
    {/each}
  </ul>
</div>

<style>
  .guides {
    max-width: 960px;
    margin: 0 auto;
    padding-top: 6rem;
    font-size: 3vw;
    color: #404040;
    font-family: "Montserrat", sans-serif;
  }
  a {
    text-decoration: none;
  }

  ul {
    display: flex;
    align-items: center;
  }

  li {
    list-style: none;
    font-style: italic;
    margin-left: 2rem;
  }
</style>
