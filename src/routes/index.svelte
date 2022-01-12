<script>
  let name = "Stranger";

  const updateTitle = () => {
    name = "Wanderer";
  };
</script>

<div class="index">
  <ul>
    <li><a href="/guide">Guide</a></li>
    <li><a href="/about">About</a></li>
  </ul>
  <h1>hello {name}</h1>
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellendus
    blanditiis, impedit corrupti sint quibusdam ad vitae autem modi quisquam
    earum dolore ipsa totam corporis omnis iste alias, ratione pariatur sit.
  </p>
  <button on:click={updateTitle}>Change Name</button>
  <input type="text" bind:value={name} />
</div>

<style>
  .index {
    max-width: 960px;
    margin: 0 auto;
    font-size: 3vw;
    color: #404040;
    font-family: "Montserrat", sans-serif;
  }
  button {
    border: 0;
    padding: 1.2rem 1.6rem 1.2rem 1.6rem;
    color: white;
    background-color: #a909e8;
    border-radius: 6rem;
    cursor: pointer;
  }
  input {
    border: 0;
    border-bottom: 1px solid #404040;
    padding: 1rem 2rem 1rem 2rem;
    font-size: 4vw;
    color: #404040;
  }

  input:focus {
    outline: none;
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
