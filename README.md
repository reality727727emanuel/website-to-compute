<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Votação - Reality</title>
<style>
body { font-family: Arial; text-align: center; }
.card { border: 1px solid #ddd; border-radius: 10px; width: 250px; margin: 10px auto; padding: 10px; }
img { width: 100%; border-radius: 10px; }
button { background: orange; color: white; border: none; padding: 10px 20px; border-radius: 5px; font-size: 16px; cursor: pointer; }
</style>
</head>
<body>
<h2>Quem você quer que fique?</h2>

<div class="card">
  <img src="nizam.jpg" alt="Nizam">
  <label><input type="radio" name="voto" value="Nizam"> Nizam</label>
</div>

<div class="card">
  <img src="saory.jpg" alt="Saory">
  <label><input type="radio" name="voto" value="Saory"> Saory</label>
</div>

<div class="card">
  <img src="tamires.jpg" alt="Tamires">
  <label><input type="radio" name="voto" value="Tamires"> Tamires</label>
</div>

<br>
<div class="h-captcha" data-sitekey="SUA_CHAVE_HCAPTCHA"></div>

<br>
<button onclick="votar()">VOTAR</button>

<script>
function votar() {
  const escolhido = document.querySelector('input[name="voto"]:checked');
  if (!escolhido) return alert('Escolha um participante!');
  alert('Voto computado com sucesso em ' + escolhido.value + '!');
}
</script>
</body>
</html>
