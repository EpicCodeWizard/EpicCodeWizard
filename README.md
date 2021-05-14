
<!doctype html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <title>Chess 0</title>
  <!--  Including the chessboardjs files:-->
  <!-- <script src="chess.js"></script>  -->
  <link rel="stylesheet" 
  href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" 
  integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO"
    crossorigin="anonymous">
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" 
  integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy"
    crossorigin="anonymous"></script>
    
  <script src="https://cdnjs.cloudflare.com/ajax/libs/chess.js/0.10.2/chess.js"></script>
  <script src="./chessboard/js/chessboard-0.3.0.min.js"></script>
  <link rel="stylesheet" href="./chessboard/css/chessboard-0.3.0.min.css">
  <style>
    .number::-webkit-inner-spin-button, 
    .number::-webkit-outer-spin-button { 
    -webkit-appearance: none; 
    margin: 0; 
    }
    #roomNumbers{
      margin: 7px;
    }
    body{
      margin: 4%
    }
  </style>

</head>

<body>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/socket.io/2.1.1/socket.io.js"></script>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
  <!-- <script src="./index.js"></script> -->
  <!-- <script>
    var socket = io();
  </script> -->
  <div class="container">
        <div id="board" style="width: 500px; margin: auto"></div>
      
      <div style="margin: auto"">
      
        <div id="player"></div>
        <div id="roomNumbers">Enter a room number between 0 and 99</div>
        <form>
          <div class="row">
            <div class="col">
              <input type="number" id="room" min="0" max="99" 
              class="form-control form-control-md number">
            </div>
            <div class="col">
              <button id="button" class="btn btn-success" onclick="connect()">Connect</button>
            </div>
          </div>
        </form>
      
        <div id="state">Join Game</div>
    </div>
    
  </div>
  

  <script src="./game.js"></script>

</body>



</html>
