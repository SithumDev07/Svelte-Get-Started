<script>
  import Logo from "$lib/logo.svelte";
</script>

<Logo name="sithum.is/about" />

<div class="index">
  <ul>
    <li><a href="/guide">Guide</a></li>
    <li><a href="/about">About</a></li>
  </ul>
  <img src="/new.jpg" alt="Profile" />
  <h1>Sithum Dashantha</h1>
  <p class="title">- IT Enthusiast -</p>
  <p class="desc">
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Non odit recusandae
    magnam, accusamus nihil asperiores et quae! Animi iusto sit rerum similique
    quis ut sequi libero maxime, dignissimos possimus natus!
  </p>
</div>

<style>
  .index {
    max-width: 960px;
    margin: 0 auto;
    font-size: 3vw;
    font-family: "Montserrat", sans-serif;
    color: #404040;
  }

  .title {
    color: blue;
    font-size: 1.3vw;
    font-style: italic;
    margin-top: -2rem;
  }

  img {
    clip-path: circle();
    width: 16vw;
    height: 16vw;
    margin-top: 5rem;
    object-fit: cover;
    margin-bottom: 0.5rem;
  }

  .desc {
    font-size: 2vw;
  }

  a {
    text-decoration: none;
  }

  ul {
    display: flex;
    align-items: center;
    margin-top: 3rem;
  }

  li {
    list-style: none;
    font-style: italic;
    margin-left: 2rem;
  }
</style>
