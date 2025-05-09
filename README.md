<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Happy Birthday, My Love</title>
  <style>
    body {
      margin: 0;
      font-family: 'Georgia', serif;
      background: linear-gradient(to bottom, #fef6f9, #e7f0ff);
      color: #5b5b5b;
      padding: 20px;
    }

    .container {
      max-width: 600px;
      margin: auto;
      background-color: #ffffffcc;
      border-radius: 20px;
      padding: 20px 25px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.08);
    }

    h1 {
      text-align: center;
      font-size: 28px;
      color: #d88c9a;
      margin-bottom: 5px;
    }

    h2 {
      text-align: center;
      font-weight: normal;
      font-size: 18px;
      color: #9e8fb2;
    }

    .heart {
      text-align: center;
      font-size: 36px;
      color: #f4a1c1;
      margin: 15px 0;
    }

    .typing {
      font-size: 16px;
      line-height: 1.7;
      white-space: pre-wrap;
      overflow-wrap: break-word;
      border-right: 2px solid #d88c9a;
      animation: blink-caret 0.75s step-end infinite;
      min-height: 150px;
    }

    @keyframes blink-caret {
      from, to { border-color: transparent; }
      50% { border-color: #d88c9a; }
    }

    .signature {
      text-align: right;
      margin-top: 30px;
      font-style: italic;
      color: #b092a5;
    }

    @media (max-width: 600px) {
      .container {
        padding: 15px 20px;
      }

      h1 {
        font-size: 24px;
      }

      h2 {
        font-size: 16px;
      }

      .typing {
        font-size: 15px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Happy Birthday, My Love</h1>
    <h2>To the one who holds my heart</h2>
    <div class="heart">💖</div>

    <div id="letter" class="typing"></div>

    <div class="signature">
      With all my love,<br/>
      [Your Name]
    </div>
  </div>

  <script>
    const text = `Today is a celebration of the most wonderful soul I know. On your birthday, I just want you to know how deeply grateful I am for you. Your presence brightens my days like the soft glow of a pastel sunrise, and your love fills my heart like a gentle breeze in spring.

Every moment with you is a memory in the making. Whether we’re laughing at something silly or simply enjoying the quiet, you make everything better just by being you.

You deserve all the joy this world has to offer—not just today, but every single day. I hope your day is as sweet as your smile and as beautiful as your heart.

Here’s to more adventures, warm embraces, and countless shared dreams. I’m so lucky to call you mine.`;

    let i = 0;
    function typeLetter() {
      if (i < text.length) {
        document.getElementById("letter").innerHTML += text.charAt(i);
        i++;
        setTimeout(typeLetter, 30); // Speed of typing (lower = faster)
      }
    }

    window.onload = typeLetter;
  </script>
</body>
</html>
