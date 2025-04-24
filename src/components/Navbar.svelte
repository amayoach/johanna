<script>
    let isMenuOpen = false;
  
    function toggleMenu() {
      isMenuOpen = !isMenuOpen;
    }
  </script>
  
  <style>
    nav {
      height: 60px;
      background-color: #000000;
      color: white;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 30px;
      font-size: 1.2rem;
      position: relative;
      font-family: "Montserrat";
      font-weight: 600;

    }
  
    .links {
      display: flex;
      gap: 15px;
    }
  
    .link {
      color: white;
      text-decoration: none;
    }
  
    .link:hover {
      text-decoration: underline;
    }
  
    /* Hamburger icon */
    .menu-icon {
      display: none;
      cursor: pointer;
      font-size: 1.5rem;
    }
  
    /* Responsive styles */
    @media (max-width: 768px) {
      .links {
        display: none; /* Hide links on small screens */
        position: absolute;
        top: 60px;
        right: 20px;
        background-color: #111;
        flex-direction: column;
        gap: 10px;
        padding: 10px;
        border-radius: 5px;
      }
  
      /* Show links if menu is open */
      .links.open {
        display: flex;
      }
  
      .menu-icon {
        display: block; /* Show menu icon on small screens */
      }
    }
  </style>
  
  <nav>
    <div>Dr Johanna Amaya-Panche</div>
  
    <!-- Menu icon for small screens -->
    <div class="menu-icon" on:click={toggleMenu}>
      ☰
    </div>
  
    <!-- Links section -->
    <div class="links {isMenuOpen ? 'open' : ''}">
      <a href="#about" class="link" on:click={() => (isMenuOpen = false)}>About</a>
      <a href="#research" class="link" on:click={() => (isMenuOpen = false)}>Research</a>
      <a href="#grants" class="link" on:click={() => (isMenuOpen = false)}>Grants</a>
      <a href="#teaching" class="link" on:click={() => (isMenuOpen = false)}>Teaching</a>
      <a href="#public" class="link" on:click={() => (isMenuOpen = false)}>Public</a>
    </div>
  </nav>
  