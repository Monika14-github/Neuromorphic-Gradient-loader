# Neuromorphic-Gradient-loader
....html.....
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
    <title>Neumorphism Gradient Loader</title>


  </head>
  <body>
    <script src="script.js"></script>
    <div class="loader">
    <span></span>
  </div>
  </body>
</html>
.....css.....
* {
  margin: 0;
  padding: 0;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background: #aab0e0;
}

.loader {
  position: relative;
  width: 200px;
  height: 200px;
  border: 4px solid #240229;
  overflow: hidden;
  border-radius: 50%;
  box-shadow: -5px -5px 5px rgba(255, 255, 255, 0.1),
    10px 10px 10px rgba(0, 0, 0, 0.4),
    inset -5px -5px 5px rgba(255, 255, 255, 0.2),
    inset 10px 10px 10px rgba(0, 0, 0, 0.4);
}

.loader:before {
  content: "";
  position: absolute;
  top: 25px;
  left: 25px;
  right: 25px;
  bottom: 25px;
  z-index: 10;
  background: #0bd8df;
  border-radius: 50%;
  border: 2px solid #69f30e;
  box-shadow: inset -2px -2px 5px rgba(255, 255, 255, 0.2),
    inset 3px 3px 5px rgba(0, 0, 0, 0.5);
}

.loader span {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background-image: linear-gradient(
    -225deg,
    #fa14c1 0%,
    #ffe700 50%,
    #fff55e 100%
  );

  filter: blur(20px);
  z-index: -1;
  animation: animate 0.5s linear infinite;
}

@keyframes animate {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}
