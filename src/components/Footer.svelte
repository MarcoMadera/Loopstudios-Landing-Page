<script>
  import Logo from "../vectors/logo.svg"
  import FacebookIcon from "../vectors/icon-facebook.svg"
  import InstagramIcon from "../vectors/icon-instagram.svg"
  import PinterestIcon from "../vectors/icon-pinterest.svg"
  import TwitterIcon from "../vectors/icon-twitter.svg"
</script>

<div class="container">
  <Logo/>
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
  <div class="social">
    <FacebookIcon/>
    <InstagramIcon/>
    <PinterestIcon/>
    <TwitterIcon/>
  </div>
  <p>© 2021 Loopstudios. All rights reserved.</p>
</div>

<style>
  .container {
    padding: 50px 20px;
    width: 100%;
    background: var(--Black);
    text-align: center;
  }
  .social {
    display: block;
    margin: 0 auto;
  }
  .social :global(svg){
    margin: 10px;
  }
  li{
    margin: 20px 0;
  }
  li a {
    text-decoration: none;
    color: var(--White);
    font-size: 15px;
    font-family: Alata;
  }
  p{
    margin-top: 10px;
    color: var(--Very-Dark-Gray);
    font-size: 16px;
    font-family: Alata;
    text-align: center;
  }
</style>