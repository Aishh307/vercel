<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chocolate Day By SHOBHIT DEV</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
</head>
<body>
    <div class="overlay"></div>
    <div class="text">
        <h2>Life is sweeter with chocolates, just like your smile! 🍫😊</h2>
        <p>I have something special for you:</p>
        <a href="new.html" class="btn">Click Here</a>
    </div>
</body>
</html>
@import url("https://fonts.google
pis.com/css?family=Bitter:700&display=swap");
*, *:before, *:after {
  position: relative;
  box-sizing: border-box;
}

html, body {
  height: 100%;
  width: 100%;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  background: #F47321;
  transform-style: preserve-3d;
  perspective: 1000px;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background: #F47321;
  font-family: 'Bitter', sans-serif;
  text-align: center;
}
.chocolate-button {
  border: none;
  background: none;
  font-size: 24px;
  font-weight: bold;
  cursor: pointer;
  margin-bottom: 20px;
}
.bar {
  display: inline-block;
  background: #754C28;
  padding: 10px 20px;
  border-radius: 5px;
  color: white;
  text-shadow: 1px 1px black;
}
.textfornext {
  font-size: 22px;
  color: rgb(255, 0, 0);
  margin-top: 100px;
}
.textfornext a {
  display: inline-block;
  background: #553310;
  color: white;
  padding: 10px 15px;
  border-radius: 5px;
  text-decoration: none;
  font-weight: bold;
  margin-top: 10px;
}
.textfornext a:hover {
  background: #8a6748;
}

.instructions {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  padding: 10rem;
  text-align: center;
  font-family: Bitter, sans-serif;
}

/* ---------------------------------- */
:root {
  --brown: #754C28;
  --brown-light: #8a6748;
  --brown-dark: #432B16;
  --brown-darker: #553310;
}

.chocolate-button {
  /* Reset button styles */
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  border: none;
  background: none;
  padding: 0;
  margin: 0;
  font-size: 10vmin;
  font-family: Bitter, cursive;
  cursor: pointer;
  transform: rotateX(10deg) rotateZ(10deg);
}
@media (min-width: 600px) {
  .chocolate-button {
    font-size: 60px;
  }
}
.chocolate-button .bar {
  border-radius: 0.3em;
  display: block;
  transition: transform 0.1s ease;
}
.chocolate-button .bar:hover, .chocolate-button .bar:focus, .chocolate-button .bar:active {
  transform: translateY(0.05em);
}
.chocolate-button .bar:before, .chocolate-button .bar:after {
  content: "";
  position: absolute;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
  border-radius: inherit;
}
.chocolate-button .bar:before {
  background-color: var(--brown);
  border: 0.35em rgba(117, 76, 40, 0.6) ridge;
  top: 0;
  z-index: 0;
}
.chocolate-button .bar:after {
  top: 0.3em;
  left: 0.3em;
  background: var(--brown-dark);
  box-shadow: inset 0 -0.05em var(--brown-darker);
}
.chocolate-button .text, .chocolate-button .bar:before, .chocolate-button .bar:after {
  transition: -webkit-clip-path 0.15s steps(3, start);
  transition: clip-path 0.15s steps(3, start);
  transition: clip-path 0.15s steps(3, start), -webkit-clip-path 0.15s steps(3, start);
  -webkit-clip-path: polygon(100% 0, 100% 100%, calc(30% + var(--x, 0) * 1px) 100%, calc(24% + var(--x, 0) * 1px) 100%, calc(7% + var(--x, 0) * 1px) 100%, calc(0% + var(--x, 0) * 1px) 100%, calc(-6% + var(--x, 0) * 1px) 100%, calc(-20% + var(--x, 0) * 1px) 100%, calc(-30% + var(--x, 0) * 1px) 100%, 0 100%, 0 0);
          clip-path: polygon(100% 0, 100% 100%, calc(30% + var(--x, 0) * 1px) 100%, calc(24% + var(--x, 0) * 1px) 100%, calc(7% + var(--x, 0) * 1px) 100%, calc(0% + var(--x, 0) * 1px) 100%, calc(-6% + var(--x, 0) * 1px) 100%, calc(-20% + var(--x, 0) * 1px) 100%, calc(-30% + var(--x, 0) * 1px) 100%, 0 100%, 0 0);
}
.chocolate-button .text {
  display: block;
  padding: 1em 0.5em;
  color: var(--brown-dark);
  opacity: 0.8;
  text-shadow: 1px 2px var(--brown-light), -1px -2px black;
}

/* ---------------------------------- */
.crumbs {
  position: absolute;
  width: 0.3em;
  height: 0.3em;
  border-radius: 50%;
  top: 0;
  left: calc(var(--x,0) * 1px);
  pointer-events: none;
  opacity: 0;
}
.crumbs:before, .crumbs:after {
  content: "";
  position: absolute;
  height: 100%;
  width: 100%;
  border-radius: inherit;
  box-shadow: -0.7469236207em 1.2466813059em var(--brown), -0.7469236207em 1.2466813059em var(--brown), -2.0202085753em 2.9480645459em var(--brown), -2.0202085753em 2.9480645459em var(--brown), 2.4328974053em 2.4983332261em var(--brown), 2.4328974053em 2.4983332261em var(--brown), -2.5822216475em 1.6743152386em var(--brown), -2.5822216475em 1.6743152386em var(--brown), -0.0778369657em 1.1914268657em var(--brown), -0.0778369657em 1.1914268657em var(--brown), 1.0855522268em 2.5192440078em var(--brown), 1.0855522268em 2.5192440078em var(--brown), 1.6360959077em 2.1229533444em var(--brown), 1.6360959077em 2.1229533444em var(--brown), -0.5531945583em 1.1120521473em var(--brown), -0.5531945583em 1.1120521473em var(--brown), 0.6857587999em 2.2473612557em var(--brown), 0.6857587999em 2.2473612557em var(--brown), -1.9868591353em 0.544609684em var(--brown), -1.9868591353em 0.544609684em var(--brown), -1.1675572309em 2.3533561717em var(--brown), -1.1675572309em 2.3533561717em var(--brown), 0.6249743959em 1.098726102em var(--brown), 0.6249743959em 1.098726102em var(--brown), 2.6847873672em 1.9232927758em var(--brown), 2.6847873672em 1.9232927758em var(--brown), 1.5414411695em 2.3332008964em var(--brown), 1.5414411695em 2.3332008964em var(--brown), -2.0487774557em 1.2274115435em var(--brown), -2.0487774557em 1.2274115435em var(--brown), -0.4448182089em 0.9870071691em var(--brown), -0.4448182089em 0.9870071691em var(--brown), -1.6576210394em 1.5560981305em var(--brown), -1.6576210394em 1.5560981305em var(--brown), 0.0171262184em 1.613514377em var(--brown), 0.0171262184em 1.613514377em var(--brown), -0.0043657671em 2.3489888032em var(--brown), -0.0043657671em 2.3489888032em var(--brown), -2.8298762657em 1.8260211373em var(--brown), -2.8298762657em 1.8260211373em var(--brown);
}
.crumbs:before {
  height: 70%;
  width: 70%;
}

/* ---------------------------------- */
.chocolate-button:focus,
.chocolate-button:active {
  outline: none;
  -webkit-animation: chomp 0.3s cubic-bezier(0.72, 0.12, 0.32, 0.96);
          animation: chomp 0.3s cubic-bezier(0.72, 0.12, 0.32, 0.96);
}
@-webkit-keyframes chomp {
  30% {
    transform: translateZ(-6vmin) rotateX(15deg) rotateZ(12deg);
  }
  70% {
    transform: translateZ(-10vmin) rotateX(0deg) rotateZ(8deg);
  }
}
@keyframes chomp {
  30% {
    transform: translateZ(-6vmin) rotateX(15deg) rotateZ(12deg);
  }
  70% {
    transform: translateZ(-10vmin) rotateX(0deg) rotateZ(8deg);
  }
}
.chocolate-button:focus .text, .chocolate-button:focus .bar:before, .chocolate-button:focus .bar:after,
.chocolate-button:active .text,
.chocolate-button:active .bar:before,
.chocolate-button:active .bar:after {
  transition: none;
  -webkit-clip-path: polygon(100% 0, 100% 100%, calc(30% + var(--x, 0) * 1px) 100%, calc(24% + var(--x, 0) * 1px) 75%, calc(7% + var(--x, 0) * 1px) 58%, calc(0% + var(--x, 0) * 1px) 65%, calc(-6% + var(--x, 0) * 1px) 45%, calc(-20% + var(--x, 0) * 1px) 51%, calc(-30% + var(--x, 0) * 1px) 100%, 0 100%, 0 0);
          clip-path: polygon(100% 0, 100% 100%, calc(30% + var(--x, 0) * 1px) 100%, calc(24% + var(--x, 0) * 1px) 75%, calc(7% + var(--x, 0) * 1px) 58%, calc(0% + var(--x, 0) * 1px) 65%, calc(-6% + var(--x, 0) * 1px) 45%, calc(-20% + var(--x, 0) * 1px) 51%, calc(-30% + var(--x, 0) * 1px) 100%, 0 100%, 0 0);
}
.chocolate-button:focus .crumbs,
.chocolate-button:active .crumbs {
  opacity: 1;
  -webkit-animation: crumbs 1.5s ease-out both;
          animation: crumbs 1.5s ease-out both;
}
@-webkit-keyframes crumbs {
  to {
    transform: translateY(100vh);
  }
}
@keyframes crumbs {
  to {
    transform: translateY(100vh);
  }
}
.chocolate-button:focus .crumbs:before,
.chocolate-button:active .crumbs:before {
  -webkit-animation: inherit;
          animation: inherit;
  -webkit-animation-name: crumbs-left;
          animation-name: crumbs-left;
  -webkit-animation-duration: 1.2s;
          animation-duration: 1.2s;
}
@-webkit-keyframes crumbs-left {
  to {
    transform: translateX(-15vw) rotate(-5deg);
  }
}
@keyframes crumbs-left {
  to {
    transform: translateX(-15vw) rotate(-5deg);
  }
}
.chocolate-button:focus .crumbs:after,
.chocolate-button:active .crumbs:after {
  -webkit-animation: inherit;
          animation: inherit;
  -webkit-animation-name: crumbs-right;
          animation-name: crumbs-right;
}
@-webkit-keyframes crumbs-right {
  to {
    transform: translateX(15vw) rotate(5deg);
  }
}
@keyframes crumbs-right {
  to {
    transform: translateX(15vw) rotate(5deg);
  }
}
<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>Chocolate Day By SHOBHIT DEV</title>
  <link rel="stylesheet" href="https://public.codepenassets.com/css/normalize-5.0.0.min.css">
<link rel="stylesheet" href="new.css">

</head>
<body>
<!-- partial:index.partial.html -->
<button class="chocolate-button">
  <div class="crumbs"></div>
  <span class="bar">
    <span class="text">Shobhit Dev</span>
  </span>
</button>

<div class="textfornext">
  <h2>I have another surprise for you! 🎁</h2> <br />  <a href="new1.html">Click Here</a></h2>
</div>

  <script  src="./script.js"></script>

</body>
</html>
body {
    background: #1e1f26;
    min-height: 100vh;
    overflow: hidden;
    display: flex;
    flex-direction: column; /* Align content vertically */
    align-items: center;
    justify-content: center;
  }
  
  svg {
    overflow: visible;
  }
  
  #chocolate_box {
    cursor: pointer;
  }
  
  #top {
    transition: transform 1s ease;
  }
  
  #chocolate_box:hover #top {
    transform: translate(40px, -25px) rotate(10deg);
    transition: transform 1s ease;
  }
  
  p {
    font-size: 20px;
    font-weight: bold;
    color: #333;
    background: #ffd1dc; /* Light pink background */
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    margin-top: 20px; /* Adds space between the chocolate box and text */
    width: 80%;
    max-width: 600px;
  }
  * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: url('background.jpg') no-repeat center center/cover;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  font-family: 'Poppins', sans-serif;
  position: relative;
}

/* Gradient Overlay */
.overlay {
  position: absolute;
  width: 100%;
  height: 100%;
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.8));
}

/* Text Styling */
.text {
  position: relative;
  color: white;
  padding: 20px;
  z-index: 2;
  max-width: 600px;
}

.text h2 {
  font-size: 2.5rem;
  font-weight: 600;
  margin-bottom: 10px;
}

.text p {
  font-size: 1.2rem;
  margin-bottom: 15px;
}

/* Button Styling */
.btn {
  text-decoration: none;
  background: #ff416c;
  color: white;
  padding: 10px 20px;
  border-radius: 25px;
  font-weight: bold;
  font-size: 1.1rem;
  display: inline-block;
  transition: all 0.3s ease-in-out;
  box-shadow: 0px 5px 15px rgba(255, 65, 108, 0.4);
}

.btn:hover {
  background: #ff4b2b;
  transform: scale(1.1);
}
