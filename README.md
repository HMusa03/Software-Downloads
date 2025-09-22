<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HM Solutions & Co. - Software Hub</title>
  <link rel="icon" type="image/png" href="images/company.logo.png">
  <style>
    :root {
      --primary: #1e4d2b;
      --secondary: #2e7d32;
      --light: #f5f7fa;
      --dark: #1d1d1f;
      --text: #444;
      --highlight: #ffd700;
    }

    body {
      margin: 0;
      font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
      background: var(--light);
      color: var(--text);
    }

    /* HEADER */
    header {
      background: var(--primary);
      color: white;
      padding: 10px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo-container {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .logo-container img {
      height: 40px;
      width: 40px;
      border-radius: 50%;
      object-fit: cover;
    }

    .logo-container h1 {
      margin: 0;
      font-size: 1.5rem;
    }

    nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
      gap: 20px;
    }

    nav ul li {
      position: relative;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      padding: 8px;
      transition: color 0.3s;
    }

    nav ul li a:hover {
      color: var(--highlight);
    }

    /* Dropdown */
    nav ul li ul {
      display: none;
      position: absolute;
      background: white;
      color: var(--text);
      min-width: 180px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      z-index: 1000;
    }

    nav ul li:hover ul {
      display: block;
    }

    nav ul li ul li a {
      color: var(--dark);
      padding: 10px;
      display: block;
    }

    nav ul li ul li a:hover {
      background: var(--light);
      color: var(--secondary);
    }

    /* HERO SECTION */
    .hero {
      padding: 60px 20px;
      text-align: center;
      background: linear-gradient(135deg, #e8f5e9, #c8e6c9);
    }

    .hero h2 {
      font-size: 2.2rem;
      margin-bottom: 15px;
      color: var(--primary);
    }

    .hero p {
      max-width: 600px;
      margin: 0 auto;
      font-size: 1.1rem;
    }

    /* FEATURED SOFTWARE */
    .section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }

    .section h3 {
      color: var(--primary);
      margin-bottom: 20px;
      border-left: 5px solid var(--highlight);
      padding-left: 10px;
    }

    .card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.1);
      margin-bottom: 25px;
    }

    .btn-download {
      display: inline-block;
      margin-top: 10px;
      padding: 12px 20px;
      font-size: 1rem;
      font-weight: bold;
      color: white;
      background: var(--primary);
      border-radius: 6px;
      text-decoration: none;
      transition: background 0.3s ease, transform 0.2s ease;
    }

    .btn-download:hover {
      background: var(--secondary);
      transform: translateY(-2px);
    }

    /* FOOTER */
    footer {
      background: var(--dark);
      color: white;
      padding: 20px;
      text-align: center;
    }

    .socials {
      margin-bottom: 10px;
    }

    .socials a {
      margin: 0 10px;
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s;
    }

    .socials a:hover {
      color: var(--highlight);
    }

    @media (max-width: 768px) {
      nav ul {
        flex-direction: column;
        gap: 10px;
      }
    }
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <div class="logo-container">
      <img src="images/company.logo.png" alt="HM Solutions Logo">
      <h1>HM Solutions & Co. (RC: 8641426)</h1>
    </div>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li>
          <a href="#">Downloads ▾</a>
          <ul>
            <li><a href="#Featured Software">Promotion Guide</a></li>
            <li><a href="#Pending Projects">Other Software (Coming Soon)</a></li>
          </ul>
        </li>
      </ul>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero">
    <h2>Welcome to HM Solutions & Co.</h2>
    <p>
      We specialize in developing innovative and practical software solutions tailored for training 
      public servants (Promotion Exam), students (UTME), Job seekers (Aptitude Test) and professional training. Explore our ready-to-use applications 
      and upcoming projects designed to simplify work and improve productivity.
    </p>
  </section>

  <!-- FEATURED SOFTWARE -->
  <section class="section">
    <h3>Featured Software</h3>
    <div class="card" id="Featured Software">
      <h4>Promotion Guide <br> This is CBT Training Software for public servants preparing for promotion exam.</h4>
      <p>
        Version: <strong>1.0.3</strong> <br>
        📦 File Size: <strong>234 MB</strong> <br>
        ⚙️ Format: <strong>Windows Setup (.exe)</strong>
      </p>
      <a class="btn-download" href="https://drive.google.com/uc?export=download&id=1Hs7aHPHAP1TBVVqYOeBSyJuLMFO-MgD5">
        ⬇ Download Now
      </a>
    </div>
  </section>

  <!-- PENDING PROJECTS -->
  <section class="section">
    <h3>Pending Projects</h3>
    <div class="card" id="Pending Projects">
      <h4>CHEW/JCHEW National Exam Training App</h4>
      <p>📌 Status: Development in progress</p>
    </div>
    <div class="card">
      <h4>Unified Tertiary Matriculation Examination (UTME-JAMB)</h4>
      <p>📌 Status: Coming soon</p>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="socials">
      <a href="mailto:hmsolutionsltd3@gmail.com">Email</a>|
      <a href="https://web.facebook.com/HMTelecoms" target="_blank">Facebook</a>|
      <a href="https://wa.me/+2348053579779" target="_blank">WhatsApp</a>|
      <a href="https://x.com/HMusa3" target="_blank">Twitter</a>|
      <a href="https://www.instagram.com/hmtelecoms0/" target="_blank">Instagram</a>|
      <a href="https://www.linkedin.com/in/hussaini-musa-68614283/" target="_blank">LinkedIn</a>
    </div>
    <p>📍 Address: Abuja, FCT, Nigeria</p>
    <p>© 2024 HM Solutions & Co. All rights reserved.</p>
  </footer>

</body>
</html>
