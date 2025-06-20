<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Roblox Login Mobile - Responsivo e Animado</title>
<link rel="icon" href="https://images.rbxcdn.com/4da3b8ff43b17378d70cb52f9a14642b-favicon.ico" />
<style>
  @import url('https://fonts.googleapis.com/css2?family=Segoe+UI&display=swap');
  * {
    box-sizing: border-box;
  }
  body {
    margin: 0;
    background-color: #121317;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    color: #d6d6d6;
    padding: 20px;
  }
  .container {
    background-color: #1a1c1f;
    border-radius: 16px;
    width: 100%;
    max-width: 400px;
    padding: 40px 32px;
    box-shadow: 0 0 35px rgba(0,0,0,0.85);
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .logo img {
    width: 140px;
    margin-bottom: 36px;
    filter: brightness(1);
  }
  input[type="text"], input[type="password"] {
    width: 100%;
    padding: 16px 18px;
    margin-bottom: 20px;
    border-radius: 12px;
    border: none;
    background: rgba(255 255 255 / 0.07);
    color: #eee;
    font-size: 17px;
    outline: none;
    transition: background-color 0.3s ease, box-shadow 0.3s ease;
    box-shadow: inset 0 0 4px rgba(0,0,0,0.5);
  }
  input[type="text"]::placeholder,
  input[type="password"]::placeholder {
    color: #888;
  }
  input[type="text"]:focus,
  input[type="password"]:focus {
    background: rgba(255 255 255 / 0.15);
    box-shadow: 0 0 6px 2px #00b06e;
  }
  button {
    width: 100%;
    padding: 16px;
    background-color: #00b06e;
    border-radius: 14px;
    border: none;
    color: white;
    font-weight: 700;
    font-size: 19px;
    cursor: pointer;
    transition: background-color 0.25s ease, box-shadow 0.25s ease;
    box-shadow: 0 4px 8px rgba(0,176,110,0.6);
  }
  button:hover {
    background-color: #009258;
    box-shadow: 0 6px 14px rgba(0,146,88,0.8);
  }
  .links {
    display: flex;
    justify-content: space-between;
    margin-top: 24px;
    font-size: 14px;
    width: 100%;
  }
  .links a {
    color: #3cd070;
    text-decoration: none;
    font-weight: 600;
  }
  .links a:hover {
    text-decoration: underline;
  }
  .alert {
    margin-top: 28px;
    font-size: 13px;
    color: #ff5555;
    font-weight: 700;
  }
  @media (max-width: 420px) {
    .container {
      padding: 32px 20px;
      width: 100%;
      max-width: 100%;
    }
  }
</style>
</head>
<body>
  <div class="container" role="main" aria-label="Roblox login form">
    <div class="logo">
      <img src="https://images.rbxcdn.com/7e14549c3a991c3e69a0c066ac960b73-logo.svg" alt="Roblox Logo" />
    </div>
    <input type="text" placeholder="Username/Email/Phone" id="username" aria-label="Username, Email or Phone" autocomplete="username" />
    <input type="password" placeholder="Password" id="password" aria-label="Password" autocomplete="current-password" />
    <button onclick="showAlert()" aria-label="Log In button">Log In</button>
    <div class="links">
      <a href="#" tabindex="0">Forgot Password or Username?</a>
      <a href="#" tabindex="0">Sign Up</a>
    </div>
    <div class="alert" id="alert" role="alert" aria-live="assertive"></div>
  </div>

  <script>
    function showAlert() {
      const alertBox = document.getElementById('alert');
      alertBox.textContent = '⚠️ Esta é uma simulação! Nunca insira seus dados em sites suspeitos.';
    }
  </script>
</body>
</html>
