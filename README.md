# For-you-3
Baby el amor que te tengo sobrepasa los limites de lo que una persona puede sentir, te amo con mi alma entera, cada latido de mi corazon dice tu nombre  y nunca se cansara de latir por ti. 
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Misión Secreta</title>
<style>
body {
  font-family: Arial, sans-serif;
  background: #111;
  color: white;
  text-align: center;
  padding: 40px;
}
button {
  padding: 12px 25px;
  margin: 10px;
  font-size: 16px;
  cursor: pointer;
  border: none;
  background: #ff4d6d;
  color: white;
  border-radius: 10px;
}
.caja {
  display: none;
  margin-top: 20px;
}
a.boton-pdf {
  display: inline-block;
  padding: 12px 25px;
  margin-top: 20px;
  font-size: 16px;
  background: #4d94ff;
  color: white;
  text-decoration: none;
  border-radius: 10px;
}
a.boton-pdf:hover {
  background: #3377ff;
}
</style>
</head>
<body>

<h1>🎮 Misión secreta</h1>
<p>Si quieres ver tu carta, completa los retos.</p>

<button onclick="nivel1()">Empezar misión</button>

<!-- Reto 1 -->
<div id="nivel1" class="caja">
  <h2>Reto 1</h2>
  <p>¿Cuánto es 4 + 4?</p>
  <input id="respuesta1" type="number">
  <button onclick="check1()">Responder</button>
</div>

<!-- Reto 2 -->
<div id="nivel2" class="caja">
  <h2>Reto 2</h2>
  <p>Elige el corazón correcto ❤️</p>
  <button onclick="wrong()">💔</button>
  <button onclick="correct()">❤️</button>
  <button onclick="wrong()">💔</button>
</div>

<!-- Carta PDF -->
<div id="carta" class="caja">
  <h1>💌 Carta desbloqueada</h1>
  <p>¡Felicidades! Has completado la misión. ❤️</p>
  <a class="boton-pdf" href="https://github.com/tuusuario/carta-juego/raw/main/carta.pdf" target="_blank">
    📄 Ver o descargar carta
  </a>
</div>

<script>
function nivel1(){
  document.getElementById("nivel1").style.display="block";
}

function check1(){
  let r = document.getElementById("respuesta1").value;
  if(r == 8){
    document.getElementById("nivel2").style.display="block";
    alert("¡Bien! Ahora el siguiente reto.");
  } else {
    alert("Incorrecto, intenta otra vez.");
  }
}

function wrong(){
  alert("Ese no es el correcto. Intenta otra vez.");
}

function correct(){
  document.getElementById("carta").style.display="block";
  alert("¡Reto completado! Tu carta está lista.");
}
</script>

</body>
</html>
