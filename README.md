<!DOCTYPE html>
<html>
<head>
  <title>Login</title>
  <meta charset="UTF-8">
</head>
<body>
  <h2>Login</h2>
  <form onsubmit="return login();">
    <label>Usuário:</label>
    <input type="text" id="username" required><br><br>
    <label>Senha:</label>
    <input type="password" id="password" required><br><br>
    <input type="submit" value="Entrar">
  </form>

  <script>
    function login() {
      const user = document.getElementById("username").value;
      const pass = document.getElementById("password").value;

      // Substitua por seus próprios dados
      if (user === "admin" && pass === "1234") {
        alert("Login bem-sucedido!");
        window.location.href = "pagina-secreta.html"; // redireciona
      } else {
        alert("Usuário ou senha incorretos.");
      }

      return false; // impede o envio do formulário
    }
  </script>
</body>
</html>
