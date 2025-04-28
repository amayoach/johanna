<div class="image-container">
  <!-- <div class="title">Dr Johanna Amaya-Panche</div> -->
  <img class="profile-image" src="./img.PNG" alt="Profile Image" />
  <div class="icons">
    <a href="https://github.com/amayoach" target="_blank">
      <img class="icon" src="github.png" alt="Github Icon" />
    </a>
    <a
      href="https://uk.linkedin.com/in/johanna-amaya-panche-phd-8775a4180"
      target="_blank"
    >
      <img class="icon" src="link.png" alt="Svelte Icon" />
    </a>
    <a href="https://orcid.org/0000-0003-0383-5559" target="_blank">
      <img class="icon" src="orcid.png" alt="ORCID Icon" />
    </a>
    <a
      href="https://scholar.google.com.co/citations?user=-dmAuMgAAAAJ&hl=en"
      target="_blank"
    >
      <img class="icon" src="google.png" alt="Google Scholar Icon" />
    </a>
    <a
      href="https://www.researchgate.net/profile/Johanna-Amaya-Panche"
      target="_blank"
    >
      <img class="icon" src="res.png" alt="Research Gate Icon" />
    </a>
    <a href="https://twitter.com/amayoap" target="_blank">
      <img class="icon" src="x.png" alt="Svelte Icon" />
    </a>
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

  .profile-image {
    width: 65%;
    border-radius: 3px;
    margin-bottom: 1rem;
  }

  .icon {
    height: 2em;
    color: white;
    font-size: 0.8rem;
    cursor: pointer;
    transition: transform 0.2s;
  }

  .icon:hover {
    transform: scale(1.2);
  }
</style>
