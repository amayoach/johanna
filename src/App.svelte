<script>
  import Navbar from './components/Navbar.svelte';
  import ProfileImage from './components/ProfileImage.svelte';
  import Content from './components/Content.svelte';
</script>

<style>
  :global(body) {
    margin: 0;
    padding: 0;
    background-color: #000; /* Black background */
    color: white;
    font-family: Arial, sans-serif;
  }

  .container {
    display: flex;
    flex-direction: column;
    height: 100vh;
    overflow: hidden;
  }

  nav {
    z-index: 1; /* Ensure navbar is above other content */
  }

  .main {
    display: flex;
    flex: 1;
    overflow: hidden;
  }

  .left {
    flex: 1 1 40%; /* Take up one-third of the width */
    max-width: 40%; /* Ensure it remains one-third on larger screens */
    position: relative;
  }

  .right {
    flex: 2 1 66.66%; /* Take up two-thirds of the width */
    overflow-y: auto;
  }

  /* Responsive styles */
  @media (max-width: 768px) {
    .main {
      flex-direction: column; /* Stack the image and content vertically */
    }

    .left {
      max-width: none; /* Reset max-width for stacking */
      flex: 0 0 auto; /* Prevent flex-grow */
    }

    .right {
      flex: 1; /* Take the remaining space */
    }
  }
</style>

<div class="container">
  <!-- Navbar at the top -->
  <Navbar />

  <!-- Main content area divided into left and right sections -->
  <div class="main">
    <div class="left">
      <ProfileImage />
    </div>
    <div class="right">
      <Content />
    </div>
  </div>
</div>
