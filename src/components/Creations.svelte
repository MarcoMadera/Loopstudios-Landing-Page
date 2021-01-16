<script>
  import Card from "./Card.svelte"
</script>

<h2>Our Creations</h2>
<div>
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
<style>
  h2{
    margin-top: 50px;
    font-family: "Josefin Sans";
    line-height: 40px;
    font-weight: 300;
    font-size: 33px;
    text-transform: uppercase;
    text-align: center;
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
  }
  @media screen and (min-width: 650px) {
    div {
      display: grid;
      grid-template-columns: repeat( auto-fit, minmax(300px, 1fr) );
    }
  }
</style>