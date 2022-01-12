<script>
  export let name = "sithum.is";
</script>

<div class="title">
  <img src="/new.jpg" alt="Logo" />
  <h1>{name}</h1>
</div>

<style>
  .title {
    max-width: 1280px;
    margin: 0 auto;
    padding-top: 2.1rem;
    font-family: "Montserrat", sans-serif;
    font-size: 0.9vw;
    color: blue;
    display: flex;
  }

  img {
    width: 5vw;
    height: 5vw;
    clip-path: circle();
    object-fit: cover;
    filter: brightness(40%);
    margin-right: 1.5rem;
  }
</style>
