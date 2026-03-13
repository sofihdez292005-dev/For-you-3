# For-you-3
Baby el amor que te tengo sobrepasa los limites de lo que una persona puede sentir, te amo con mi alma entera, cada latido de mi corazon dice tu nombre  y nunca se cansara de latir por ti. 
<!DOCTYPE html>
<html>
<head>
<title>Misión Cartita</title>
<style>
body{
font-family: Arial;
background:#111;
color:white;
text-align:center;
padding:40px;
}

button{
padding:12px 25px;
margin:10px;
font-size:16px;
cursor:pointer;
border:none;
background:#ff4d6d;
color:white;
border-radius:10px;
}

.caja{
display:none;
margin-top:20px;
}
</style>
</head>

<body>

<h1>🎮 Misión Cartita</h1>
<p>Si quieres ver tu carta debes completar los retos. TE AMO</p>

<button onclick="nivel1()">Empezar misión</button>

<div id="nivel1" class="caja">
<h2>Reto 1</h2>
<p>¿Cuánto es 4 + 285?</p>
<input id="respuesta1">
<button onclick="check1()">Responder</button>
</div>

<div id="nivel2" class="caja">
<h2>Reto 2</h2>
<p>Elige el corazón correcto</p>

<button onclick="wrong()">💔</button>
<button onclick="correct()">❤️</button>
<button onclick="wrong()">💔</button>

</div>

<div id="carta" class="caja">
<h1>💌 Carta desbloqueada</h1>
<p>
Si llegaste hasta aquí, te debo decir que vales mas de lo que te podes imaginar, yo se lo que es estar en el cielo porque lo siento cuando estoy en tus brazos.❤️
</p>
</div>

<script>

function nivel1(){
document.getElementById("nivel1").style.display="block";
}

function check1(){
let r = document.getElementById("respuesta1").value;

if(r == 8){
document.getElementById("nivel2").style.display="block";
}else{
alert("Incorrecto, intenta otra vez");
}
}

function wrong(){
alert("Ese no es el correcto");
}

function correct(){
document.getElementById("carta").style.display="block";
}

</script>

</body>
</html>
