<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>My Simple HTML Page</title>
  <!-- Simple inline styles for clarity -->
  <style>
    body { font-family: Arial, sans-serif; line-height: 1.6; margin: 20px; }
    header { margin-bottom: 16px; }
    nav a { margin-right: 10px; text-decoration: none; }
    .card { border: 1px solid #ddd; padding: 12px; border-radius: 8px; display:inline-block; }
    footer { margin-top: 20px; color: #666; font-size: 0.9em; }
  </style>
</head>
<body>

  <header>
    <h1>Welcome to My Simple Page</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#features">Features</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>About</h2>
      <p>This is a very basic HTML5 page showing common elements: headings, paragraphs, lists, an image, a link, and a little JavaScript.</p>
    </section>

    <section id="features">
      <h2>Features</h2>
      <ul>
        <li>Semantic sections (&lt;header&gt;, &lt;main&gt;, &lt;footer&gt;)</li>
        <li>Simple CSS inside &lt;style&gt;</li>
        <li>Small interactive button using JavaScript</li>
      </ul>

      <div class="card">
        <h3>Try this</h3>
        <p>Click the button to see a greeting.</p>
        <button id="greetBtn">Say Hello</button>
      </div>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <p>Visit <a href="https://example.com" target="_blank" rel="noopener">example.com</a> for more info.</p>
      <!-- image placeholder (replace src with an actual image path if you have one) -->
      <img src="https://via.placeholder.com/300x150?text=Placeholder+Image" alt="Placeholder" />
    </section>
  </main>

  <footer>
    &copy; <span id="year"></span> My Simple Page
  </footer>

  <script>
    // small JS for interactivity
    document.getElementById('greetBtn').addEventListener('click', function () {
      alert('Hello — welcome to your simple HTML page!');
    });

    // set current year in footer
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>

</body>
</html>