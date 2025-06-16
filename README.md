# ViNi-Enterprise1.github.io

<html lang="pl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ViNi | Strony internetowe na zamówienie</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #f4f4f4;
      color: #333;
      scroll-behavior: smooth;
    }
    header {
      background: #111;
      color: white;
      padding: 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2.5em;
      color: #3ecf8e;
    }
    nav {
      background: #222;
      display: flex;
      justify-content: center;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      padding: 15px 20px;
      display: block;
    }
    nav a:hover {
      background: #3ecf8e;
      color: #111;
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
    }
    .hero {
      text-align: center;
    }
    .hero h2 {
      font-size: 2em;
      margin-bottom: 10px;
    }
    .services, .about, .contact {
      background: white;
      margin-top: 30px;
      border-radius: 10px;
      padding: 40px 20px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .services h3, .about h3, .contact h3 {
      margin-top: 0;
      color: #3ecf8e;
    }
    .service-list {
      list-style: none;
      padding: 0;
    }
    .service-list li {
      padding: 10px 0;
      border-bottom: 1px solid #ddd;
    }
    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0 20px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 1em;
    }
    form button {
      background: #3ecf8e;
      color: #111;
      border: none;
      padding: 12px 20px;
      font-weight: bold;
      cursor: pointer;
      border-radius: 5px;
    }
    form button:hover {
      background: #32b87a;
    }
    footer {
      background: #111;
      color: #aaa;
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
    }
  </style>
</head>
<body>

  <header>
    <h1>ViNi</h1>
    <p>Profesjonalne strony internetowe na zamówienie</p>
  </header>

  <nav>
    <a href="#services">Usługi</a>
    <a href="#about">O nas</a>
    <a href="#contact">Kontakt</a>
  </nav>

  <section class="hero">
    <h2>Twoja strona, Twoje zasady.</h2>
    <p>W ViNi projektujemy szybkie, nowoczesne i responsywne strony dostosowane do Twoich potrzeb.</p>
  </section>

  <section id="services" class="services">
    <h3>Nasze usługi</h3>
    <ul class="service-list">
      <li>Projektowanie stron internetowych na zamówienie</li>
      <li>Optymalizacja mobilna</li>
      <li>Strony docelowe dla kampanii</li>
      <li>Portfolio, blogi i sklepy internetowe</li>
      <li>Utrzymanie i aktualizacje</li>
    </ul>
  </section>

  <section id="about" class="about">
    <h3>O ViNi</h3>
    <p>ViNi to firma freelancer specjalizująca się w tworzeniu wysokiej jakości, czystych i skutecznych stron internetowych dla osób prywatnych, startupów i firm. Niezależnie czy potrzebujesz prostej strony docelowej czy pełnej witryny, ViNi dostarczy efekt, który świetnie wygląda i działa.</p>
  </section>

  <section id="contact" class="contact">
    <h3>Kontakt</h3>
    <form id="contactForm">
      <input type="text" id="name" placeholder="Twoje imię" required />
      <input type="email" id="email" placeholder="Twój email" required />
      <textarea id="message" rows="5" placeholder="Twoja wiadomość" required></textarea>
      <button type="submit">Wyślij wiadomość</button>
    </form>
    <p id="formMsg" style="color: green;"></p>
  </section>

  <footer>
    &copy; 2025 ViNi. Wszelkie prawa zastrzeżone.
  </footer>

  <script>
    document.getElementById('contactForm').addEventListener('submit', function(e) {
      e.preventDefault();

      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();
      const msg = document.getElementById('formMsg');

      if (!name || !email || !message) {
        msg.style.color = 'red';
        msg.textContent = "Proszę wypełnić wszystkie pola.";
        return;
      }

      msg.style.color = 'green';
      msg.textContent = `Dziękujemy ${name}, wkrótce się z Tobą skontaktujemy!`;

      this.reset();
    });
  </script>

</body>
</html>
