<script>
  import Logo from "../vectors/logo.svg"
  import HamburgerMenu from "../vectors/icon-hamburger.svg"
  import CloseIcon from "../vectors/icon-close.svg"

  let modalIsOpen = false;
  function handleClick() {
    modalIsOpen = !modalIsOpen;
  }
</script>

<div class="hero">
  <nav>
    <Logo class="logo"/>
    <div>
      <div class="menu">
        <ul>
          <li>
            <a href="#about">About</a>
          </li>
          <li>
            <a href="#careers">Careers</a>
          </li>
          <li>
            <a href="#events">Events</a>
          </li>
          <li>
            <a href="#products">Products</a>
          </li>
          <li>
            <a href="#support">Support</a>
          </li>
        </ul>
      </div>
      <button on:click={handleClick} class="hamburger-menu">
        {#if modalIsOpen}
          <CloseIcon class="icon"/>
        {:else}
          <HamburgerMenu class="icon"/>
        {/if}
      </button>
      <div class="modal" style={`display: ${modalIsOpen ? "block": "none"};`}>
        <div class="modalList">
          <ul>
            <li>
              <a href="#about">About</a>
            </li>
            <li>
              <a href="#careers">Careers</a>
            </li>
            <li>
              <a href="#events">Events</a>
            </li>
            <li>
              <a href="#products">Products</a>
            </li>
            <li>
              <a href="#support">Support</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
  <div class="hero__title__container">
    <div class="hero__content">
      <h1>Immersive experiences that deliver</h1>
    </div>

  </div>
</div>

<svelte:head>
   {#if modalIsOpen}
      <style>
         body {
            overflow: hidden;
         }
      </style>
   {/if}
</svelte:head>	

<style>
  .modal{
    height: 100vh;
    width: 100vw;
    background: var(--Black);
    position: absolute;
    top: 0;
    left: 0;
    z-index: 1;
  }
  .modalList {
    display: flex;
    align-items: center;
    height: 100vh;
    width: 100%;
  }
  :global(.icon),:global(.logo){
    position: relative;
    z-index: 9999;
  }
  .modal ul{
    margin: 0 20px;
  }
  .modal li{
    list-style: none;
    margin: 30px 0;
  }
  .modal li a {
    text-decoration: none;
    color: var(--White);
    font-size: 30px;
    font-family: "Josefin Sans";
    text-transform: uppercase;
  }
  h1 {
    color: var(--White);
    font-family: "Josefin Sans";
    line-height: 40px;
    font-weight: 300;
    font-size: 40px;
    word-spacing: 100vw;
    text-transform: uppercase;
  }
  nav {
    padding: 40px 24px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  a {
    text-decoration: none;
    color: var(--White);
  }
  .menu ul {
    display: flex;
  }
  .menu li {
    padding: 10px;
    list-style: none;
  }
  a:hover, a:focus{
    text-align:center;
    padding-bottom:10px;
    background: linear-gradient(to right, rgb(255, 255, 255), rgb(255, 255, 255) 100%) no-repeat bottom center;
    background-size: 25px 2px;
  }
  .hero__title__container{
    width: 100%;
    height: calc(650px - 112px);
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .hero__content{
    display: flex;
    justify-content: center;
    align-items: center;
    width: calc(100% - 40px);
    padding: 20px;
    border: 2px solid var(--White);
  }
  .hero {
    width: 100%;
    height: 650px;
    background-image: url("/assets/images/mobile/image-hero.jpg");
    background-repeat: no-repeat;
    background-size: cover;
  }
  .menu{
    display: none;
  }
  .hamburger-menu{
    background: none;
    border:none;
  }
  @media screen and (min-width: 650px){
    nav {
      padding: 30px 50px;
    }
    h1 {
      font-size: 60px;
      line-height: 60px;
    }
    .hero{
      background-image: url("/assets/images/desktop/image-hero.jpg");
    }
    .hero__content{
      margin: 80px 50px;
      height: 280px;
      width: 650px;
    }
    .menu{
      display: flex;
    }
    .hamburger-menu{
      display: none;
    }
    .hero__title__container{
      justify-content: start;
    }
  }
  @media screen and (min-width: 1024px){
    nav {
      padding: 25px 160px;
    }
    nav {
      height: 111px;
    }
    .hero__content{
    margin: 160px;
    }
  }
</style>