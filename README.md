<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Online PRMS Style Login</title>
  <style>
    body {
      margin: 0;
      background-color: #4178a2;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }

    .top-content {
      text-align: center;
      margin-bottom: 20px;
    }

    .logo-image {
      width: 120px;
      height: auto;
      display: block;
      margin: 0 auto 10px;
      user-select: none;
    }

    .logo {
      font-size: 2rem;
    }

    .logo span {
      color: #D22500;
      font-weight: bold;
    }

    .login-card, .container {
      background-color: white;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      width: 350px;
      text-align: center;
    }

    .hidden {
      display: none;
    }

    h1, h2 {
      color: #1dcbe1;
      margin-bottom: 1.5rem;
    }

    input[type="text"],
    input[type="password"] {
      width: 90%;
      padding: 0.8rem;
      margin-bottom: 1rem;
      border: none;
      background-color: #e4e9f0;
      border-radius: 5px;
    }

    button {
      background-color: #0dcbe1;
      color: white;
      border: none;
      padding: 0.7rem 1.5rem;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 1rem;
      font-weight: bold;
    }

    button:hover {
      background: #3F94BF;
      color: #000;
    }

    .btn-tutorial {
      display: block;
      width: 100%;
      margin-top: 2rem;
    }

    .remember {
      display: flex;
      align-items: center;
      justify-content: start;
      margin-top: 0.5rem;
      font-size: 0.9rem;
      color: #555;
    }

    .remember input {
      margin-right: 0.5rem;
    }
    .bgimg1 {
  width: 100%;
  height: auto;
  border-radius: 10px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
  margin-bottom: 1rem;
}

  </style>
</head>
<body>
  <div class="top-content">
    <img src="https://i.imgur.com/Hv6oV8E.png" alt="Logo" class="logo-image">
    <div class="logo">Online <span>PRMS</span></div>
  </div>

  <!-- Login Section -->
  <div class="login-card container" id="home">
    <h1>Sign In</h1>
    <input type="text" placeholder="Username/Email">
    <input type="password" placeholder="Password">
    <button onclick="showSection('dashboard')">LOGIN</button>

    <div class="remember">
      <input type="checkbox" id="remember">
      <label for="remember">Remember</label>
    </div>
    <button class="btn-tutorial">WATCH ONLINE PAIS TUTORIALS</button>
  </div>

  <!-- Dashboard Section -->
  <!-- Dashboard Section -->
<div class="container hidden" id="dashboard">
  <h2>HELLO SABI NI ALDEN RICHARDS!</h2>
  <div style="margin-bottom: 1rem;">
    <img class="bgimg1" src="https://i.imgur.com/275TImJ.jpeg" alt="bgimg">
  </div>
  <p>IZA PRANKS! HAHAHAHAHAHAHAHAHAHA</p>
  <button onclick="showSection('home')">Logout</button>
</div>

  <script>
    function showSection(id) {
      document.querySelectorAll('.container').forEach(el => el.classList.add('hidden'));
      document.getElementById(id).classList.remove('hidden');
    }
  </script>
</body>
</html>
