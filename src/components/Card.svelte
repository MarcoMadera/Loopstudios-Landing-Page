<script>
  export let img; 
  export let title;
</script>

<a href="#{title.replaceAll(" ", "-")}" class="Card">
  <picture>
    <source srcSet="assets/images/desktop/{img}" media="(min-width: 650px)" />
    <img src="assets/images/mobile/{img}" alt={title}>
  </picture>
  <h3>{title}</h3>
</a>

<style>
  .Card{
    display: block;
    position: relative;
    margin: 0 auto;
  }
  img{
    max-width: 100%;
    display: block;
    margin: 20px auto;
    filter: brightness(0.7);
    transition: .4s ease;
  }
  h3{
    position: absolute;
    bottom: 15px;
    left: 22px;
    color: var(--White);
    font-size: 24px;
    font-family: "Josefin Sans";
    line-height: 30px;
    font-weight: 300;
    text-transform: uppercase;
    width: 130px;
    text-shadow: 0px 0px 30px #000;
    transition: .4s ease;
  }
  .Card:hover img, .Card:focus img {
      opacity: 0.4;
  }
  .Card:hover h3, .Card:focus h3 {
    color: var(--Black);
  }
  @media screen and (min-width: 650px){
    .Card {
      margin: 0;
      width: 256px;
      height: 450px;
      height: max-content;
      box-shadow: 0px 0px 7px 2px rgba(0, 0, 0, 0.03);
      text-decoration: none;
    }
    img {
      margin: 0;
    }
  }
</style>