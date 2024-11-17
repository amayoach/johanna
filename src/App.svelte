<script>
  import Navbar from './components/Navbar.svelte';
  import ProfileImage from './components/ProfileImage.svelte';
  import Content from './components/Content.svelte';
</script>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    background-color: #000;
    color: white;
    font-family: Arial, sans-serif;
  }

  .container {
    display: flex;
    flex-direction: column;
    height: 100vh;
    overflow: hidden;
  }

  .main {
    display: flex;
    flex: 1;
    overflow: hidden;
  }

  .left {
    flex: 1 1 40%;
    max-width: 40%;
    overflow-y: auto; /* Enable scrolling for image section */
  }

  .right {
    flex: 2 1 60%;
    overflow-y: auto;
  }

  /* Responsive styles for small screens */
  @media (max-width: 768px) {
    .main {
      flex-direction: column;
      overflow-y: auto; /* Enable scrolling for entire content */
    }

    .left, .right {
      max-width: 100%;
      flex: none;
    }
  }
</style>

<div class="container">
  <Navbar />
  <div class="main">
    <div class="left">
      <ProfileImage />
    </div>
    <div class="right">
      <Content />
    </div>
  </div>
</div>