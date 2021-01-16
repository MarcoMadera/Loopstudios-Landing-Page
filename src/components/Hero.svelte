<script>
  import Logo from "../vectors/logo.svg"
</script>

<div class="hero">
  <nav>
    <Logo />
    <div class="hamburger-menu">
      <span></span>
      <span></span>
      <span></span>
    </div>
  </nav>
  <div class="hero__content">
    <h1>Immersive experiences that deliver</h1>
  </div>
</div>

<style>
  h1 {
    margin: 20px;
    padding: 20px;
    border: 2px solid var(--White);
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
  .hero__content{
    height: calc(650px - 112px);
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .hamburger-menu span{
    display: block;
    width: 30px;
    height: 2px;
    background: #fff;
  }
  .hamburger-menu span:nth-of-type(1),
  .hamburger-menu span:nth-of-type(2){
    margin-bottom: 7px;
  }
  .hero {
    width: 100%;
    height: 650px;
    background-image: url("/assets/images/mobile/image-hero.jpg");
    background-repeat: no-repeat;
    background-size: cover;
  }
</style>