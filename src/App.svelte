<script>
  export let dark;

  function handleToggle() {
    dark = !dark;
  }
</script>

<style>
  .container {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .toggle {
    border: none;
    outline: none;
    border-radius: 5px;
    padding: 10px;
    color: white;
  }
  .toggle:hover {
    cursor: pointer;
  }
  .dark {
    background-color: #3b5998;
    color: white;
  }
  .light {
    background-color: #ffffff;
    color: black;
  }
</style>

<div class="container {dark ? 'dark' : 'light'}">
  <button class="toggle {dark ? 'light' : 'dark'}" on:click={handleToggle}>
    Toggle background
  </button>
</div>
