<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Leviathan Project</title>
  <style>
    /* GENERAL */
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(to bottom, #0b0b0b, #1a1a1a);
      color: #e0e0e0;
      text-align: center;
      overflow-x: hidden;
    }

    /* ANIMATED WAVES BACKGROUND */
    body::before {
      content: "";
      position: fixed;
      top: 0;
      left: 0;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle at 50% 50%, rgba(10,10,30,0.2), transparent 70%);
      animation: wave 20s linear infinite;
      z-index: -1;
    }

    @keyframes wave {
      0% { transform: translate(0,0) rotate(0deg); }
      50% { transform: translate(-50px, 20px) rotate(2deg); }
      100% { transform: translate(0,0) rotate(0deg); }
    }

    /* HEADER */
    header {
      padding: 50px 20px 20px 20px;
    }

    #logo {
      width: 200px;
      height: auto;
      margin-bottom: 20px;
      animation: pulse 3s infinite;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.05); }
      100% { transform: scale(1); }
    }

    h1 {
      font-size: 2.2em;
      letter-spacing: 2px;
      margin-bottom: 10px;
    }

    /* NAVIGATION */
    nav {
      margin: 30px 0;
    }

    nav a {
      display: inline-block;
      text-decoration: none;
      color: #a5a5ff;
      background-color: rgba(255,255,255,0.05);
      padding: 12px 25px;
      margin: 10px;
      border-radius: 8px;
      font-weight: bold;
      transition: 0.3s;
    }

    nav a:hover {
      background-color: #3030ff;
      color: #fff;
      box-shadow: 0 0 15px #3030ff;
    }

    section {
      max-width: 700px;
      margin: 20px auto;
      text-align: left;
      line-height: 1.6;
      padding: 0 20px;
    }

    /* QR CODE PLACEHOLDER */
    .qr-placeholder {
      display: block;
      width: 150px;
      height: 150px;
      background-color: #111;
      margin: 20px auto;
      border-radius: 12px;
      border: 3px solid #555;
      line-height: 150px;
      color: #888;
      font-weight: bold;
      position: relative;
    }

    .qr-placeholder::after {
      content: "";
      position: absolute;
      top: -5px;
      left: -5px;
      width: 160px;
      height: 160px;
      border: 2px dashed #444;
      border-radius: 14px;
      animation: glow 2s infinite alternate;
    }

    @keyframes glow {
      from { box-shadow: 0 0 5px #222; }
      to { box-shadow: 0 0 15px #444; }
    }

    footer {
      margin-top: 50px;
      padding: 20px;
      font-size: 0.9em;
      color: #888;
    }
  </style>
</head>
<body>
  <header>
    <img src="logo.png" alt="Leviathan Logo" id="logo">
    <h1>Child of God: Leviathan Project</h1>
    <nav>
      <a href="#verify">Verify Authenticity</a>
      <a href="#about">About the Abyss</a>
      <a href="#findus">Find Us</a>
    </nav>
  </header>

  <section id="verify">
    <h2>Verify Authenticity</h2>
    <p>Scan the QR code on your product to confirm it is an authentic Leviathan Project item.</p>
    <div class="qr-placeholder">QR Code</div>
  </section>

  <section id="about">
    <h2>About the Abyss</h2>
    <p>
      Leviathan Project is inspired by ancient mythic creatures of the deep. 
      Every product is crafted to honor the mysterious and the powerful forces of the abyss.
    </p>
  </section>

  <section id="findus">
    <h2>Find Us</h2>
    <p>
      Instagram: <a href="https://instagram.com/cglp" target="_blank">@cglp</a><br>
      Shopee: <a href="#" target="_blank">Leviathan Project Official</a><br>
      Contact: <a href="mailto:leviathan@example.com">leviathan@example.com</a>
    </p>
  </section>

  <footer>
    &copy; 2025 Leviathan Project. All rights reserved.
  </footer>
</body>
</html>
