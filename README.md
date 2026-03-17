# Search-App-Hub
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Daily Dashboard</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #ffecd2 0%, #fcb69f 100%);
      text-align: center;
      color: #333;
    }
    header {
      background-color: rgba(255, 255, 255, 0.8);
      padding: 30px 20px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.2);
    }
    h1 {
      font-size: 2.5rem;
      margin: 0;
      color: #ff6f61;
    }
    .search-box {
      margin: 30px auto;
    }
    .search-box input {
      width: 60%;
      padding: 15px;
      border: none;
      border-radius: 30px;
      font-size: 18px;
      outline: none;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    .search-box button {
      padding: 15px 25px;
      border: none;
      border-radius: 30px;
      background-color: #ff6f61;
      color: #fff;
      font-size: 18px;
      margin-left: 10px;
      cursor: pointer;
      box-shadow: 0 2px 8px rgba(0,0,0,0.2);
      transition: background-color 0.3s;
    }
    .search-box button:hover {
      background-color: #e55b4a;
    }
    .app-icons {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 40px;
      margin: 40px auto;
      max-width: 1000px;
    }
    .app-icons a {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-decoration: none;
      font-size: 34px;
      color: #fff;
      width: 100px;
      height: 100px;
      background: linear-gradient(135deg, #6e8efb, #a777e3);
      border-radius: 20px;
      justify-content: center;
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .app-icons a:hover {
      transform: scale(1.1);
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
    .icon-label {
      font-size: 14px;
      margin-top: 8px;
      color: #fff;
    }
  </style>
</head>
<body>
  <header>
    <h1>Search & App Hub</h1>
    <div class="search-box">
      <input type="text" id="searchInput" placeholder="Search the web...">
      <button onclick="performSearch()">Search</button>
    </div>
  </header>
  <section class="app-icons">
    <a href="https://www.google.com" target="_blank" title="Google">
      <i class="fab fa-google"></i>
      <span class="icon-label">Google</span>
    </a>
    <a href="https://www.youtube.com" target="_blank" title="YouTube">
      <i class="fab fa-youtube"></i>
      <span class="icon-label">YouTube</span>
    </a>
    <a href="https://mail.google.com" target="_blank" title="Gmail">
      <i class="fas fa-envelope"></i>
      <span class="icon-label">Gmail</span>
    </a>
    <a href="https://web.whatsapp.com" target="_blank" title="WhatsApp">
      <i class="fab fa-whatsapp"></i>
      <span class="icon-label">WhatsApp</span>
    </a>
    <a href="https://www.instagram.com" target="_blank" title="Instagram">
      <i class="fab fa-instagram"></i>
      <span class="icon-label">Instagram</span>
    </a>
    <a href="https://www.facebook.com" target="_blank" title="Facebook">
      <i class="fab fa-facebook"></i>
      <span class="icon-label">Facebook</span>
    </a>
    <a href="https://www.twitter.com" target="_blank" title="Twitter">
      <i class="fab fa-twitter"></i>
      <span class="icon-label">Twitter</span>
    </a>
  </section>  <script>
    function performSearch() {
      const query = document.getElementById("searchInput").value;
      if (query.trim() !== '') {
        const url = `https://www.google.com/search?q=${encodeURIComponent(query)}`;
        window.open(url, '_blank');
      }
    }
  </script></body>
</html>
