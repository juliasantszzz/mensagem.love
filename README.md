<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Frase en corazon Encoded</title>
  <style>
    @import url("https://fonts.googleapis.com/css?family=Gaegu");
    body {
      background-color: #dec5e1;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: "Gaegu", cursive;
      overflow: hidden;
    }
    .heart {
      width: 120px;
      height: 120px;
      position: absolute;
      display: flex;
      justify-content: center;
      align-items: center;
      transition: all 1s 0.2s ease;
      opacity: 1;
    }
    .heart:hover {
      width: 180px;
      height: 180px;
      cursor: pointer;
    }
    .heart.anime {
      animation: heartbeat 0.8s 0.2s ease infinite alternate;
      position: absolute;
      cursor: auto;
    }
    @keyframes heartbeat {
      0% {
        width: 120px;
        height: 120px;
        transition: all 1s 0.2s ease;
      }
      100% {
        width: 140px;
        height: 140px;
        transition: all 1s 0.2s ease;
      }
    }
    .heart:before,
    .heart:after {
      position: absolute;
      background-color: #ef6c57;
      content: "";
      width: 50%;
      height: 75%;
    }
    .heart:before {
      transform: rotate(-45deg);
      border-radius: 400px 400px 0px 100px;
      left: 16%;
    }
    .heart:after {
      transform: rotate(45deg);
      border-radius: 400px 400px 100px 0px;
      right: 16%;
    }
    .heart.active {
      width: 500px;
      height: 500px;
      animation: none !important;
      transition: all 1s 0.2s ease;
      cursor: auto;
      transform: rotate(10deg), rotate(0deg);
      position: absolute;
    }
    .heart:hover.active {
      width: 500px;
      height: 500px;
    }
    .heart .title {
      opacity: 1;
      color: #f2f2f2;
      position: absolute;
      transition: all 0.8s 0.5s ease;
      z-index: 1;
      text-align: center;
      margin: 0 auto;
      margin-top: -3%;
      animation: title 3s 1s ease infinite;
    }
    @keyframes title {
      0%, 25%, 100% {
        transform: rotate(0deg);
      }
      5%, 15% {
        transform: rotate(5deg);
      }
      10%, 20% {
        transform: rotate(-5deg);
      }
    }
    .heart.active .title {
      opacity: 0;
      transition: all 0.8s 0s ease;
    }
    .heart .message {
      opacity: 0;
      color: #f2f2f2;
      transition: all 0.2s 0s ease;
      text-align: center;
      margin: 0 auto;
      width: 80%;
      margin-top: -20%;
      font-size: 16px;
      z-index: 1;
    }
    .heart.active .message {
      opacity: 1;
      z-index: 1;
      margin-top: -10%;
      transition: all 1s 0.5s ease;
    }
    .hearts {
      width: 100%;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      opacity: 1;
    }
    .heart2,
    .heart3,
    .heart4 {
      width: 20px;
      height: 20px;
      position: absolute;
      opacity: 0;
      z-index: -1;
      transition: all 1s ease;
    }
    .heart2.active {
      opacity: 1;
      animation: floatHearts1 2s 0.2s ease;
    }
    .heart3.active {
      opacity: 1;
      animation: floatHearts2 2s 0.2s ease;
    }
    .heart4.active {
      opacity: 1;
      animation: floatHearts3 2s 0.2s ease;
    }
    @keyframes floatHearts1 {
      0% {
        width: 20px;
        height: 20px;
        left: 50%;
        top: 60%;
        transform: rotate(0deg);
      }
      50% {
        top: 30%;
      }
      100% {
        width: 50px;
        height: 50px;
        left: -20%;
        top: 20%;
        transform: rotate(-40deg);
      }
    }
    @keyframes floatHearts2 {
      0% {
        width: 20px;
        height: 20px;
        right: 50%;
        top: 60%;
        transform: rotate(0deg);
      }
      100% {
        width: 100px;
        height: 100px;
        right: 0%;
        top: -20%;
        transform: rotate(40deg);
      }
    }
    @keyframes floatHearts3 {
      0% {
        width: 20px;
        height: 20px;
        right: 50%;
        top: 50%;
        transform: rotate(0deg);
      }
      50% {
        top: 100%;
      }
      100% {
        width: 80px;
        height: 80px;
        right: 0%;
        top: 110%;
        transform: rotate(90deg);
      }
    }
    .heart2:before,
    .heart2:after,
    .heart3:before,
    .heart3:after,
    .heart4:before,
    .heart4:after {
      position: absolute;
      background-color: #ef6c57;
      content: "";
      width: 50%;
      height: 90%;
      z-index: 2;
    }
    .heart2:before,
    .heart3:before,
    .heart4:before {
      transform: rotate(-45deg);
      border-radius: 400px 400px 0px 100px;
      left: 10%;
    }
    .heart2:after,
    .heart3:after,
    .heart4:after {
      transform: rotate(45deg);
      border-radius: 400px 400px 100px 0px;
      right: 10%;
    }
    .custom-button {
      display: none;
      margin-top: 20px; /* Espaço acima do botão */
      padding: 10px 20px;
      background-color: #ef6c57;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div class="heart">
    <p class="title">Clique aqui...</p>
    <p class="message">Daniel... <br>
      Para o homem incrível que você é<br>
      minha gratidão pela felicidade que está trazendo na minha vida<br>
      e que eu seja capaz de te fazer feliz<br>
      na mesma proporção. e sim, <br> 
      estou te amando.❤<br><br>
      &hearts; &hearts; &hearts;
    </p>
  </div>
  <div class="heart anime"></div>
  <div class="hearts">
    <div class="heart2"></div>
    <div class="heart3"></div>
    <div class="heart4"></div>
  </div>

  <!-- Botão "Olha só" -->
  <button class="custom-button" onclick="window.location.href='file:///C:/Users/julia.souza/teste%204.html'">Olha só</button>

  <script> 
    var heart = document.querySelector('.heart'),
        animeHeart = document.querySelector('.heart.anime'),
        hearts = document.querySelector('.hearts'),
        heart2 = document.querySelector('.heart2'),
        heart3 = document.querySelector('.heart3'),
        heart4 = document.querySelector('.heart4'),
        button = document.querySelector('.custom-button');

    heart.addEventListener('click', function () {
      heart.classList.add('active');
      animeHeart.classList.add('active');
      hearts.classList.add('active');
      heart2.classList.add('active');
      heart3.classList.add('active');
      heart4.classList.add('active');

      // Mostrar o botão "Olha só" após o clique no coração
      button.style.display = 'block';
    });
  </script>
</body>
</html>


<script> 
 var heart = document.querySelector('.heart'),
    reload = document.querySelector('.reload'),
    hearts = document.querySelector('.hearts'),
    allHearts = document.querySelectorAll('.hearts div'),
   heartAnime = document.querySelector('.heart.anime')
    

heart.addEventListener('click', animation);

reload.addEventListener('click', refresh)


function animation() {
   heart.classList.add("active");
   reload.setAttribute("style", "opacity: 1; cursor: pointer; pointer-events: auto;  ");
   heartAnime.style.opacity = "0";

   allHearts.forEach(function(element) {
      element.classList.add("active");
   })
}

function refresh() {
  heart.classList.remove("active");
      reload.setAttribute("style", "opacity: 0; pointer-events: none;");
   heartAnime.style.opacity = "1";;

   allHearts.forEach(function(element) {
      element.classList.remove("active");
   })
   
}
   /* by encodedmabel 
 linktr.ee/mabelolivera10
   */
</script>



<style>
/* by encoded mabel 
    linktr.ee/mabelolivera10
    */
    
    @import url("https://fonts.googleapis.com/css?family=Gaegu");
    .about {
      position: fixed;
      z-index: 10;
      bottom: 10px;
      right: 10px;
      width: 40px;
      height: 40px;
      display: flex;
      justify-content: flex-end;
      align-items: flex-end;
      transition: all 0.2s ease;
    }
    
    
    body {
      background-color: #dec5e1;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: "Gaegu", cursive;
      overflow: hidden;
    }
    
    /* reload button */
    .reload {
      position: absolute;
      top: 0;
      z-index: 1;
      color: #010503;
      transition: all 0.5s 0.5s ease;
      width: auto;
      height: auto;
      opacity: 0;
      text-align: center;
      display: flex;
      justify-content: center;
      align-items: center;
      top: 0;
    }
    
    .reload:hover {
      color: white;
      top: 5px;
    }
    
    .reload:after {
      background-color: #ef6c57;
      content: "";
      width: 0;
      height: 2px;
      opacity: 1;
      border-radius: 30px;
      position: absolute;
      bottom: -4px;
      z-index: -1;
      transition: width 0.5s 0.5s ease, height 0.5s 0s ease;
    }
    
    .reload:hover:after {
      transition: width 0.5s 0s ease, height 0.5s 0.5s ease;
      width: calc(100% + 30px);
      height: calc(100% + 10px);
    }
    
    /* elements container */
    .content {
      display: flex;
      justify-content: center;
      align-items: center;
    }
    
    /* main heart */
    .heart {
      width: 120px;
      height: 120px;
      position: absolute;
      display: flex;
      justify-content: center;
      align-items: center;
      transition: all 1s 0.2s ease;
      opacity: 1;
    }
    
    .heart:hover {
      width: 180px;
      height: 180px;
      cursor: pointer;
    }
    
    /* background heart - animated */
    .heart.anime {
      animation: heartbeat 0.8s 0.2s ease infinite alternate;
      position: absolute;
      cursor: auto;
    }
    
    @keyframes heartbeat {
      0% {
        width: 120px;
        height: 120px;
        transition: all 1s 0.2s ease;
      }
      100% {
        width: 140px;
        height: 140px;
        transition: all 1s 0.2s ease;
      }
    }
    /* elements that compose the heart */
    .heart:before,
    .heart:after {
      position: absolute;
      background-color: #ef6c57;
      content: "";
      width: 50%;
      height: 75%;
    }
    
    .heart:before {
      transform: rotate(-45deg);
      border-radius: 400px 400px 0px 100px;
      left: 16%;
    }
    
    .heart:after {
      transform: rotate(45deg);
      border-radius: 400px 400px 100px 0px;
      right: 16%;
    }
    
    /* active state to grow the heart */
    .heart.active {
      width: 500px;
      height: 500px;
      animation: none !important;
      transition: all 1s 0.2s ease;
      cursor: auto;
      transform: rotate(10deg), rotate(0deg);
      position: absolute;
    }
    
    .heart:hover.active {
      width: 500px;
      height: 500px;
    }
    
    /* title - click */
    .heart .title {
      opacity: 1;
      color: #f2f2f2;
      position: absolute;
      transition: all 0.8s 0.5s ease;
      z-index: 1;
      text-align: center;
      margin: 0 auto;
      margin-top: -3%;
      animation: title 3s 1s ease infinite;
    }
    
    @keyframes title {
      0%, 25%, 100% {
        transform: rotate(0deg);
      }
      5%, 15% {
        transform: rotate(5deg);
      }
      10%, 20% {
        transform: rotate(-5deg);
      }
    }
    /* active state that hide the title */
    .heart.active .title {
      opacity: 0;
      transition: all 0.8s 0s ease;
    }
    
    /* message */
    .heart .message {
      opacity: 0;
      color: #f2f2f2;
      transition: all 0.2s 0s ease;
      text-align: center;
      margin: 0 auto;
      width: 80%;
      margin-top: -20%;
      font-size: 16px;
      z-index: 1;
      
    }
    
    /* active state that show the message */
    .heart.active .message {
      opacity: 1;
      z-index: 1;
      margin-top: -10%;
      transition: all 1s 0.5s ease;
    }
    
    /* floating hearts */
    .hearts {
      width: 100%;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      opacity: 1;
    }
    
    .heart2,
    .heart3,
    .heart4 {
      width: 20px;
      height: 20px;
      position: absolute;
      opacity: 0;
      z-index: -1;
      transition: all 1s ease;
    }
    
    .heart2.active {
      opacity: 1;
      animation: floatHearts1 2s 0.2s ease;
    }
    
    .heart3.active {
      opacity: 1;
      animation: floatHearts2 2s 0.2s ease;
    }
    
    .heart4.active {
      opacity: 1;
      animation: floatHearts3 2s 0.2s ease;
    }
    
    @keyframes floatHearts1 {
      0% {
        width: 20px;
        height: 20px;
        left: 50%;
        top: 60%;
        transform: rotate(0deg);
      }
      50% {
        top: 30%;
      }
      100% {
        width: 50px;
        height: 50px;
        left: -20%;
        top: 20%;
        transform: rotate(-40deg);
      }
    }
    @keyframes floatHearts2 {
      0% {
        width: 20px;
        height: 20px;
        right: 50%;
        top: 60%;
        transform: rotate(0deg);
      }
      100% {
        width: 100px;
        height: 100px;
        right: 0%;
        top: -20%;
        transform: rotate(40deg);
      }
    }
    @keyframes floatHearts3 {
      0% {
        width: 20px;
        height: 20px;
        right: 50%;
        top: 50%;
        transform: rotate(0deg);
      }
      50% {
        top: 100%;
      }
      100% {
        width: 80px;
        height: 80px;
        right: 0%;
        top: 110%;
        transform: rotate(90deg);
      }
    }
    .heart2:before,
    .heart2:after,
    .heart3:before,
    .heart3:after,
    .heart4:before,
    .heart4:after {
      position: absolute;
      background-color: #ef6c57;
      content: "";
      width: 50%;
      height: 90%;
      z-index: 2;
    }
    
    .heart2:before,
    .heart3:before,
    .heart4:before {
      transform: rotate(-45deg);
      border-radius: 400px 400px 0px 100px;
      left: 10%;
    }
    
    .heart2:after,
    .heart3:after,
    .heart4:after {
      transform: rotate(45deg);
      border-radius: 400px 400px 100px 0px;
      right: 10%;
    }
</style>
