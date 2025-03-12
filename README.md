<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ledcrip - Python Coder</title>
  <style>
    /* General Styles */
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #1e3c72, #2a5298);
      color: #fff;
      overflow-x: hidden;
    }

    .container {
      max-width: 100%;
      padding: 20px;
      box-sizing: border-box;
      text-align: center;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
      animation: fadeIn 2s ease-in-out;
    }

    p {
      font-size: 1.2rem;
      line-height: 1.6;
      animation: slideUp 1.5s ease-in-out;
    }

    .highlight {
      color: #ffd700;
      font-weight: bold;
    }

    /* Animations */
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes slideUp {
      from { transform: translateY(20px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes glow {
      0% { text-shadow: 0 0 5px #ffd700; }
      50% { text-shadow: 0 0 20px #ffd700; }
      100% { text-shadow: 0 0 5px #ffd700; }
    }

    /* Button Styles */
    .btn {
      display: inline-block;
      margin-top: 20px;
      padding: 10px 20px;
      font-size: 1rem;
      color: #fff;
      background: #ff6f61;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s ease, transform 0.3s ease;
      animation: glow 2s infinite;
    }

    .btn:hover {
      background: #ff3b2f;
      transform: scale(1.1);
    }

    /* Responsive Design */
    @media (max-width: 600px) {
      h1 {
        font-size: 2rem;
      }

      p {
        font-size: 1rem;
      }

      .btn {
        font-size: 0.9rem;
        padding: 8px 16px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Ledcrip</h1>
    <p>
      Hi, I'm <span class="highlight">Ledcrip</span>, a passionate Python coder with over <span class="highlight">3 years of experience</span>. 
      I specialize in creating efficient, scalable, and elegant solutions using Python. 
      From web development to data analysis, I love turning ideas into reality through code.
    </p>
    <button class="btn" onclick="alert('Hello from Ledcrip!')">Say Hello</button>
  </div>

  <script>
    // Optional: Add more interactive animations or functionality here
    document.querySelector('h1').addEventListener('mouseover', () => {
      document.querySelector('h1').style.animation = 'glow 1s infinite';
    });

    document.querySelector('h1').addEventListener('mouseout', () => {
      document.querySelector('h1').style.animation = 'fadeIn 2s ease-in-out';
    });
  </script>
</body>
</html>
