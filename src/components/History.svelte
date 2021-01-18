<img src="/assets/images/mobile/image-interactive.jpg" alt="Guy playing in VR"/>
<div class="History__container">
  <div class="History__content">
    <h2>The leader in interactive VR</h2>
    <p>
      Founded in 2011, Loopstudios has been producing world-class virtual reality 
      projects for some of the best companies around the globe. Our award-winning 
      creations have transformed businesses through digital experiences that bind 
      to their brand.
    </p>
  </div>
</div>
<style>
  img{
    width: 100%;
    min-height: 225px;
    max-width: 650px;
    margin: 0 auto;
    display: block;
  }
  h2 {
    margin-top: 50px;
    font-family: "Josefin Sans";
    line-height: 40px;
    font-weight: 300;
    font-size: 33px;
    text-transform: uppercase;
    text-align: center;
    margin-bottom: 15px;
  }
  p {
    text-align: center;
    color: var(--Dark-Gray);
    margin: 0 20px;
    line-height: 23px;
  }
  div {
    padding: 0;
  }
  @media screen and (min-width: 1200px){
    .History__container{
      position: relative;
      width: 100%;
      height: 100px;
    }
    h2{
      font-size: 45px;
      line-height: 45px;
    }
    img{
      margin: 0 164px;
      width: 730px;
      height: 500px;
    }
    .History__content{
      position: absolute;
      width: 650px;
      background-color: var(--White);
      padding: 100px 50px;
      margin-top: -300px;
      right: 0px;
      bottom: 0;
    }
    h2,p{
      text-align: left;
      margin: 0;
    }
  }
</style>