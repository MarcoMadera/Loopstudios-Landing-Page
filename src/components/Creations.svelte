<script>
  import Card from "./Card.svelte"
</script>

<div class="Creations">
  <h2>Our Creations</h2>
  <div class="cards">
    <Card img="image-deep-earth.jpg" title="deep earth"/>
    <Card img="image-night-arcade.jpg" title="night arcade"/>
    <Card img="image-soccer-team.jpg" title="soccer team vr"/>
    <Card img="image-grid.jpg" title="the grid"/>
    <Card img="image-from-above.jpg" title="from up above vr"/>
    <Card img="image-pocket-borealis.jpg" title="pocket borealis"/>
    <Card img="image-curiosity.jpg" title="the curiosity"/>
    <Card img="image-fisheye.jpg" title="make it fisheye"/>
  </div>
  <a href="#all">See all</a>
</div>
<style>
  h2{
    font-family: "Josefin Sans";
    line-height: 40px;
    font-weight: 300;
    font-size: 33px;
    text-transform: uppercase;
    text-align: center;
    margin-top: 0;
    margin-bottom: 15px;
  }
  a {
    width: 150px;
    height: 40px;
    border: 2px solid var(--Black);
    color: var(--Black);
    text-transform: uppercase;
    letter-spacing: 4px;
    text-align: center;
    font-size: 20px;
    display: block;
    margin: 0 auto;
    padding: 5px;
    text-decoration: none;
    transition: .4s ease;
  }
  a:hover, a:focus {
    background: var(--Black);
    color: var(--White);
  }
  .Creations {
    margin-top: 50px;
  }
  @media screen and (min-width: 650px) {
    .Creations {
      display: grid;
      grid-template-columns: 1fr 150px;
      grid-template-rows: 70px 1fr;
    }
    .cards {
      display: grid;
    grid-template-columns: repeat(auto-fit, 256px);
    column-gap: 30px;
    row-gap: 30px;
    justify-content: space-between;
    grid-area: cards;
    grid-area: 2 / 1 / 3 / 3;
    }
    h2{
      text-align: left;
      grid-area: title;
      grid-area: 1 / 1 / 2 / 2;
      margin: 0;
    }
    a{
      grid-area: button;
      margin: 0;
      grid-area: 1 / 2 / 2 / 3;
    }
  }
</style>