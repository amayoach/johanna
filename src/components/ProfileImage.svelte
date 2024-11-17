<div class="image-container">
  <div class="title">Dr Johanna Amaya-Panche</div>
  <img src="./img.PNG" alt="Profile Image" />
  <div class="icons">
    <img
      class="icon"
      src="./src/assets/github.png"
      alt="Svelte Icon"
      style="height: 2em;"
    />
    <img
      class="icon"
      src="./src/assets/link.png"
      alt="Svelte Icon"
      style="height: 2em;"
    />
    <img
      class="icon"
      src="./src/assets/orcid.png"
      alt="Svelte Icon"
      style="height: 2em;"
    />
    <img
      class="icon"
      src="./src/assets/google.png"
      alt="Svelte Icon"
      style="height: 2em;"
    />
    <img
      class="icon"
      src="./src/assets/res.png"
      alt="Svelte Icon"
      style="height: 2em;"
    />
    <img
      class="icon"
      src="./src/assets/x.png"
      alt="Svelte Icon"
      style="height: 2em;"
    />
  </div>
</div>

<style>
  .image-container {
    font-family: "Montserrat";
    font-weight: 500;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column; /* Stack elements vertically */
    align-items: center;
    justify-content: center;
    background-color: #000000;
  }

  .title {
    color: white; /* Ensure the title is visible against the black background */
    font-size: 1.5rem;
    margin-bottom: 1rem; /* Space between the title and the image */
  }

  img {
    width: 65%;
    border-radius: 3px;
    margin-bottom: 1rem; /* Space between the image and the icons */
  }

  .icons {
    display: flex;
    gap: 1rem; /* Add spacing between icons */
  }

  .icon {
    color: white;
    font-size: 0.8rem;
    cursor: pointer;
    transition: transform 0.2s;
  }

  .icon:hover {
    transform: scale(1.2); /* Slight zoom effect on hover */
  }
</style>
