<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="Content-Security-Policy" content="default-src 'self'; script-src 'self'; style-src 'self' 'unsafe-inline'; connect-src 'self'; img-src 'self' data:; frame-src https://www.messenger.com https://www.tiktok.com https://www.instagram.com https://www.twitter.com https://web.whatsapp.com;">
  <title>Unified Social Hub</title>
  <script>
    // Simulated local storage for device-based login detection
    const userId = "user123"; // Replace with a dynamic user ID if needed
    const isDeviceRecognized = localStorage.getItem(`deviceRecognized_${userId}`);

    if (!isDeviceRecognized) {
      const password = prompt("This device is not recognized. Please enter your password:");
      if (password !== "your-secure-password") {
        alert("Incorrect password. Access denied.");
        window.location.href = "about:blank"; // Block further access
      } else {
        localStorage.setItem(`deviceRecognized_${userId}`, 'true');
        alert("Device recognized. Welcome!");
      }
    } else {
      alert("Welcome back! Device recognized.");
    }
  </script>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #6a11cb, #2575fc);
      color: white;
      margin: 0;
      padding: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      text-align: center;
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 30px;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
    }

    p {
      font-size: 1.2rem;
      margin-bottom: 40px;
      max-width: 600px;
    }

    .button-container {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }

    .button {
      display: inline-block;
      padding: 15px 30px;
      font-size: 1.2rem;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      transition: transform 0.3s, box-shadow 0.3s;
      font-weight: bold;
    }

    .button:hover {
      transform: scale(1.1);
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
    }

    .messenger {
      background-color: #0084ff;
    }

    .tiktok {
      background-color: #000;
    }

    .instagram {
      background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285aeb 90%);
    }

    .twitter {
      background-color: #1da1f2;
    }

    .whatsapp {
      background-color: #25d366;
    }

    footer {
      margin-top: 40px;
      font-size: 0.9rem;
      color: rgba(255, 255, 255, 0.8);
    }
  </style>
</head>
<body>
  <h1>Welcome to the Unified Social Hub</h1>
  <p>Your one-stop destination to access all your favorite social platforms. Click on any app below to get started!</p>
  <div class="button-container">
    <a href="https://www.messenger.com" target="_blank" rel="noopener noreferrer" class="button messenger">Open Messenger</a>
    <a href="https://www.tiktok.com" target="_blank" rel="noopener noreferrer" class="button tiktok">Open TikTok</a>
    <a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="button instagram">Open Instagram</a>
    <a href="https://www.twitter.com" target="_blank" rel="noopener noreferrer" class="button twitter">Open Twitter</a>
    <a href="https://web.whatsapp.com" target="_blank" rel="noopener noreferrer" class="button whatsapp">Open WhatsApp</a>
  </div>
  <footer>
    &copy; mediahub.anish <instagram>https://www.instagram.com/aneeshgiree555/#</instagram>
  </footer>
</body>
</html# mediahub
