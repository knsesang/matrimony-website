<script>
  let menuOpen = false;

  function toggleMenu() {
    menuOpen = !menuOpen;
  }
</script>

<header>
  <div class="container">
    <div class="logo">
      <h1>인연맺음</h1>
      <p>AI 기반 결혼중개 플랫폼</p>
    </div>
    <nav class="nav-desktop">
      <a href="#features">특징</a>
      <a href="#architecture">아키텍처</a>
      <a href="#technology">기술</a>
      <a href="#roadmap">로드맵</a>
      <a href="#contact">문의</a>
    </nav>
    <button class="menu-toggle" on:click={toggleMenu}>☰</button>
  </div>
  {#if menuOpen}
    <nav class="nav-mobile">
      <a href="#features" on:click={() => menuOpen = false}>특징</a>
      <a href="#architecture" on:click={() => menuOpen = false}>아키텍처</a>
      <a href="#technology" on:click={() => menuOpen = false}>기술</a>
      <a href="#roadmap" on:click={() => menuOpen = false}>로드맵</a>
      <a href="#contact" on:click={() => menuOpen = false}>문의</a>
    </nav>
  {/if}
</header>

<style>
  header {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo h1 {
    font-size: 1.8rem;
    font-weight: bold;
    margin: 0;
  }

  .logo p {
    font-size: 0.9rem;
    opacity: 0.9;
    margin: 0;
  }

  .nav-desktop {
    display: flex;
    gap: 2rem;
  }

  .nav-desktop a {
    color: white;
    font-weight: 500;
    transition: opacity 0.3s;
  }

  .nav-desktop a:hover {
    opacity: 0.8;
    text-decoration: none;
  }

  .menu-toggle {
    display: none;
    background: none;
    border: none;
    color: white;
    font-size: 1.5rem;
    cursor: pointer;
  }

  .nav-mobile {
    display: none;
    flex-direction: column;
    gap: 1rem;
    padding: 1rem;
    background: rgba(0, 0, 0, 0.1);
  }

  .nav-mobile a {
    color: white;
    font-weight: 500;
  }

  @media (max-width: 768px) {
    .nav-desktop {
      display: none;
    }

    .menu-toggle {
      display: block;
    }

    .nav-mobile {
      display: flex;
    }

    .logo h1 {
      font-size: 1.4rem;
    }
  }
</style>

