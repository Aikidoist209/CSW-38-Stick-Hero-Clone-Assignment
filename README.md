# CSW-38-Stick-Hero-Clone-Assignment



function drawBackground() {
  const backgroundImage = new Image();
  backgroundImage.src = "New-background.jpg";

  const scrolloffset = (sceneOffset * backgroundSpeedMultiplier) % canvasWidth;

  ctx.drawImage(backgroundImage, -scrolloffset, 0, canvasWidth, canvasHeight);
  ctx.drawImage(backgroundImage, -scrolloffset + canvasWidth, 0, window.innerWidth, window.innerHeight);


  <div id="youtube-card">
  How to create a Stick Hero game with JavaScript and HTML Canvas
</div>

<a id="youtube" href="https://youtu.be/eue3UdFvwPo" target="_top">
  <span>See how this game was made</span>
</a>



#perfect {
  position: absolute;
  opacity: 0;
  transition: opacity 2s;
}

#youtube,
#youtube-card {
  display: none;
}

@media (min-height: 425px) {
  /** Youtube logo by https://codepen.io/alvaromontoro */
  #youtube {
    z-index: 2;
    display: block;
    width: 100px;
    height: 70px;
    position: absolute;
    bottom: 20px;
    left: 20px;
    background: red;
    border-radius: 50% / 11%;
    transform: scale(0.8);
    transition: transform 0.5s;
  }

  #youtube:hover,
  #youtube:focus {
    transform: scale(0.9);
  }

  #youtube::before {
    content: "";
    display: block;
    position: absolute;
    top: 7.5%;
    left: -6%;
    width: 112%;
    height: 85%;
    background: red;
    border-radius: 9% / 50%;
  }

  #youtube::after {
    content: "";
    display: block;
    position: absolute;
    top: 20px;
    left: 40px;
    width: 45px;
    height: 30px;
    border: 15px solid transparent;
    box-sizing: border-box;
    border-left: 30px solid white;
  }

  #youtube span {
    font-size: 0;
    position: absolute;
    width: 0;
    height: 0;
    overflow: hidden;
  }

  #youtube:hover + #youtube-card {
    display: block;
    position: absolute;
    bottom: 12px;
    left: 10px;
    padding: 25px 25px 25px 130px;
    width: 300px;
    background-color: white;
  }
}
