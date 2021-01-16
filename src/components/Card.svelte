<script>
  export let img; 
  export let title;
</script>

<div>
  <picture>
    <source srcSet="assets/images/desktop/{img}" media="(min-width: 650px)" />
    <img src="assets/images/mobile/{img}" alt={title}>
  </picture>
  <h3>{title}</h3>
</div>

<style>
  img{
    max-width: 100%;
    display: block;
    margin: 20px auto;
    filter: brightness(0.7);
  }
  div{
    position: relative;
    margin: 0 auto;
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
  }
  @media screen and (min-width: 650px){
    div {
      width: max-content;
    }
  }
</style>