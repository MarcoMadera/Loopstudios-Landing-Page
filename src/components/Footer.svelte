<script>
  import Logo from "../vectors/logo.svg"
  import FacebookIcon from "../vectors/icon-facebook.svg"
  import InstagramIcon from "../vectors/icon-instagram.svg"
  import PinterestIcon from "../vectors/icon-pinterest.svg"
  import TwitterIcon from "../vectors/icon-twitter.svg"
</script>

<div class="container">
  <Logo class="logo"/>
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
    <a href="#facebook">
      <FacebookIcon/>
    </a>
    <a href="#instragram">
      <InstagramIcon/>
    </a>
    <a href="#pinterest">
      <PinterestIcon/>
    </a>
    <a href="#twitter">
      <TwitterIcon/>
    </a>
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
  .social a{
    display: inline-flex;
    margin: 0 10px;
  }
  li{
    list-style: none;
    margin: 20px 0;
  }
  li a {
    text-decoration: none;
    color: var(--White);
    font-size: 15px;
    font-family: Alata;
  }
  a:hover, a:focus{
    text-align:center;
    padding-bottom:10px;
    background: linear-gradient(to right, rgb(255, 255, 255), rgb(255, 255, 255) 100%) no-repeat bottom center;
    background-size: 25px 2px;
  }
  p{
    margin-top: 10px;
    color: var(--Very-Dark-Gray);
    font-size: 16px;
    font-family: Alata;
    text-align: center;
  }
  @media screen and (min-width: 650px){
    .container {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-template-rows: repeat(2, 1fr);
      grid-column-gap: 0px;
      grid-row-gap: 0px;
    }
    :global(.logo) {
      grid-area: 1 / 1 / 2 / 2;
    }
    .social{
      margin: 0 0 0 auto;
      grid-area: 1 / 2 / 2 / 3;
    }
    ul {
      grid-area: 2 / 1 / 3 / 2;
      display: flex;
    }
    li {
    margin: 10px;
    }
    li:first-child {
      margin: 10px 10px 10px 0;
    }
    p {
      grid-area: 2 / 2 / 3 / 3;
      text-align: right;
    }
  }
  @media screen and (min-width:1024px){
    .container{
      padding: 50px 160px;
    }
  }
</style>