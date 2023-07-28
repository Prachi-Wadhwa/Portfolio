<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <style>
    body {
      background-color: black;
    }
    .first {
      /* background-color: aquamarine; */
      background-image: url("https://images.unsplash.com/photo-1522252234503-e356532cafd5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8ZGV2ZWxvcGVyfGVufDB8fDB8fHww&w=1000&q=80");
      background-repeat: no-repeat;
      background-size: 100%;
      margin: 0%;
      /* margin: 10%; */
      /* padding: 10%; */
      color: darkgray;
    }
    .intro {
      font-size: 5rem;
      margin: 10%;
      padding: 10%;
    }
    .intro1 {
      font-size: 2.3rem;
      margin: 10%;
      padding: 10%;
    }
    .box-container {
      align-items: center;
      display: flex;
      flex-direction: row;
      justify-content: space-around;
      padding: 70px 20px;
      width: 100%;
      flex-wrap: wrap;
    }

    /* @media screen and (min-width:1380px) {
  .box-container {
    flex-direction: row
  }
} */

    .box-item {
      position: relative;
      -webkit-backface-visibility: hidden;
      width: 380px;
      margin-bottom: 35px;
      max-width: 100%;
      padding: 5%;
    }

    .flip-box {
      -ms-transform-style: preserve-3d;
      transform-style: preserve-3d;
      -webkit-transform-style: preserve-3d;
      perspective: 1000px;
      -webkit-perspective: 1000px;
    }

    .flip-box-front,
    .flip-box-back {
      background-size: cover;
      background-position: center;
      border-radius: 8px;
      min-height: 600px;
      -ms-transition: transform 0.7s cubic-bezier(0.4, 0.2, 0.2, 1);
      transition: transform 0.7s cubic-bezier(0.4, 0.2, 0.2, 1);
      -webkit-transition: transform 0.7s cubic-bezier(0.4, 0.2, 0.2, 1);
      -webkit-backface-visibility: hidden;
      backface-visibility: hidden;
    }

    .flip-box-front {
      -ms-transform: rotateY(0deg);
      -webkit-transform: rotateY(0deg);
      transform: rotateY(0deg);
      -webkit-transform-style: preserve-3d;
      -ms-transform-style: preserve-3d;
      transform-style: preserve-3d;
    }

    .flip-box:hover .flip-box-front {
      -ms-transform: rotateY(-180deg);
      -webkit-transform: rotateY(-180deg);
      transform: rotateY(-180deg);
      -webkit-transform-style: preserve-3d;
      -ms-transform-style: preserve-3d;
      transform-style: preserve-3d;
    }

    .flip-box-back {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;

      -ms-transform: rotateY(180deg);
      -webkit-transform: rotateY(180deg);
      transform: rotateY(180deg);
      -webkit-transform-style: preserve-3d;
      -ms-transform-style: preserve-3d;
      transform-style: preserve-3d;
    }

    .flip-box:hover .flip-box-back {
      -ms-transform: rotateY(0deg);
      -webkit-transform: rotateY(0deg);
      transform: rotateY(0deg);
      -webkit-transform-style: preserve-3d;
      -ms-transform-style: preserve-3d;
      transform-style: preserve-3d;
    }

    .flip-box .inner {
      position: absolute;
      left: 0;
      width: 100%;
      padding: 40px 20px 20px;
      outline: 1px solid transparent;
      -webkit-perspective: inherit;
      perspective: inherit;
      z-index: 2;

      transform: translateY(-0%) translateZ(60px) scale(0.94);
      -webkit-transform: translateY(-0%) translateZ(60px) scale(0.94);
      -ms-transform: translateY(-0%) translateZ(60px) scale(0.94);
      top: 0%;
      /* font-size: 2rem; */
    }

    .flip-box-header {
      font-size: 34px;
    }

    .flip-box p {
      font-size: 20px;
      line-height: 1.5em;
    }

    .flip-box-img {
      margin-top: 25px;
    }

    .flip-box-button {
      background-color: transparent;
      border: 2px solid #fff;
      border-radius: 2px;
      color: #fff;
      cursor: pointer;
      font-size: 20px;
      font-weight: bold;
      margin-top: 25px;
      padding: 15px 20px;
      text-transform: uppercase;
    }
    .fa {
      color: black;
      height: 50px;
      width: 50px;
    }
    .icons {
      margin-top: 50%;
      padding: 50px;
      margin: 30px;
    }
    footer {
      background-color: lightgray;
      margin-top: 80px;
      margin-bottom: 0px;
      height: 150px;
      text-align: center;
      font-size: 2rem;
    }
    .container {
      display: flex;
    }
  </style>
  <body>
    <div class="first">
      <p class="intro">Hello, I'm Prachi Wadhwa.<br />I'm a designer.</p>
      <p class="intro1">
        I am a beginner and wish to achieve my highest potent!
      </p>
    </div>
    <div class="container">
      <div class="box-item">
        <div class="flip-box">
          <div
            class="flip-box-front"
            style="
              background-image: url('https://thumbs.dreamstime.com/b/education-concept-vertical-25835396.jpg');
            "
          >
            <div class="inner color-white"></div>
          </div>
          <div class="flip-box-back" style="background: #4477dd">
            <!-- <div class="liquid">
            <img src="https://www.milkshake.co/img/Liquid%20Drop2x.png" class="img-fluid" />
          </div> -->
            <div class="inner color-white">
              <p>Senior Secondary Education</p>
              <pre>   G.N.K. Sr. Sec. School</pre>
              <pre>   2019-2021</pre>
              <pre>   91.8%</pre>
              <p>Graduation</p>
              <pre>   B.E. CSE</pre>
              <pre>   Chitkara University</pre>
              <pre>   2021-25</pre>
              <pre>   9.35 cgpa</pre>
            </div>
          </div>
        </div>
      </div>
      <div class="box-item">
        <div class="flip-box">
          <div
            class="flip-box-front"
            style="
              background-image: url('https://img.freepik.com/free-photo/top-view-skills-written-note-with-notepad-light-background-job-office-school-copybook-college-business-colors_179666-18276.jpg');
            "
          >
            <div class="inner color-white"></div>
          </div>
          <div class="flip-box-back" style="background: #4477dd">
            <!-- <div class="liquid">
            <img src="./img/Liquid Drop2x.png" class="img-fluid" />
          </div> -->
            <div class="inner color-white">
              <ul style="font-size: 2rem">
                <li>HTML</li>
                <li>CSS</li>
                <li>JS</li>
                <li>Python</li>
                <li>C++</li>
                <li>C</li>
                <li>Java</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="box-item">
        <div class="flip-box">
          <div
            class="flip-box-front"
            style="
              background-image: url('https://www.i-scoop.eu/wp-content/uploads/2015/01/User-experience.gif');
            "
          >
            <div class="inner color-white"></div>
          </div>
          <div class="flip-box-back" style="background: #4477dd">
            <!-- <div class="liquid">
            <img src="./img/Liquid Drop2x.png" class="img-fluid" />
          </div> -->
            <div class="inner color-white">
              <p>Beginner.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <footer>
      <div class="icons">
        <a href="https://www.instagram.com/miss_wadhwa_16/"
          ><i class="fa-brands fa-instagram fa fa-lg"></i></a
        >&nbsp;&nbsp; <i class="fa-brands fa-twitter fa fa-lg"></i>&nbsp;&nbsp;
        <a href="https://www.linkedin.com/in/prachi-wadhwa-3b4882232/"
          ><i class="fa-brands fa-linkedin fa fa-lg"></i></a
        >&nbsp;&nbsp;
        <a href="https://web.whatsapp.com/"
          ><i class="fa-brands fa-whatsapp fa fa-lg"></i
        ></a>
      </div>
    </footer>
  </body>
  <script
    src="https://kit.fontawesome.com/2cdc036eb4.js"
    crossorigin="anonymous"
  ></script>
</html>
