<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Future of Digital Marketing Portfolio</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
    background: #f7f9fc;
    color: #333;
  }
  header {
    background: #0d6efd;
    color: #fff;
    padding: 1.5rem 2rem;
    text-align: center;
  }
  header h1 {
    margin: 0;
    font-weight: 700;
  }
  nav {
    display: flex;
    background: #0a58ca;
    justify-content: center;
  }
  nav button {
    background: none;
    border: none;
    padding: 1rem 2rem;
    color: #fff;
    font-size: 1rem;
    cursor: pointer;
    transition: background 0.3s ease;
  }
  nav button:hover, nav button.active {
    background: #083d9a;
  }
  section {
    padding: 2rem;
    max-width: 900px;
    margin: 0 auto;
    display: none;
  }
  section.active {
    display: block;
  }
  h2 {
    color: #0d6efd;
    margin-bottom: 1rem;
  }
  ul {
    line-height: 1.6;
  }
  .project-card {
    background: white;
    padding: 1rem 1.5rem;
    margin: 1rem 0;
    border-radius: 8px;
    box-shadow: 0 0 8px rgba(0,0,0,0.1);
  }
  .project-card h3 {
    margin-top: 0;
  }
  .contact-form {
    max-width: 400px;
    margin-top: 1.5rem;
  }
  .contact-form label {
    display: block;
    margin: 1rem 0 0.3rem 0;
  }
  .contact-form input, .contact-form textarea {
    width: 100%;
    padding: 0.6rem;
    border-radius: 4px;
    border: 1px solid #ccc;
    resize: vertical;
  }
  .contact-form button {
    margin-top: 1rem;
    background: #0d6efd;
    color: white;
    padding: 0.7rem 1.2rem;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    font-weight: 600;
  }
  footer {
    text-align: center;
    padding: 1.5rem;
    background: #e9ecef;
    margin-top: 3rem;
    font-size: 0.9rem;
    color: #555;
  }
</style>
</head>
<body>

<header>
  <h1>Future of Digital Marketing Portfolio</h1>
  <p>Showcasing Skills, Trends & Projects for 2025</p>
</header>

<nav>
  <button class="tab-btn active" data-tab="about">About</button>
  <button class="tab-btn" data-tab="trends">Trending Skills</button>
  <button class="tab-btn" data-tab="projects">Projects</button>
  <button class="tab-btn" data-tab="contact">Contact</button>
</nav>

<section id="about" class="active">
  <h2>About Me</h2>
  <p>I am a digital marketing enthusiast focused on the future of marketing through AI, social commerce, and immersive technologies. My goal is to leverage the latest trends and tech to build engaging marketing campaigns that deliver results.</p>
</section>

<section id="trends">
  <h2>Trending Skills for 2025</h2>
  <ul>
    <li>AI-powered marketing automation and personalization</li>
    <li>Social commerce integration on platforms like Instagram and TikTok</li>
    <li>Data privacy-focused marketing strategies</li>
    <li>Use of AR/VR for immersive brand experiences</li>
    <li>Predictive analytics for market trend anticipation</li>
  </ul>
</section>

<section id="projects">
  <h2>Selected Projects</h2>
  <div class="project-card">
    <h3>AI Chatbot Campaign</h3>
    <p>Developed and implemented AI chatbot technology for customer interaction, resulting in a 40% increase in engagement and faster issue resolution.</p>
  </div>
  <div class="project-card">
    <h3>Social Commerce Launch</h3>
    <p>Integrated shoppable posts with Instagram for a retail client, boosting in-app purchases by 35% within the first quarter.</p>
  </div>
  <div class="project-card">
    <h3>Immersive AR Experience</h3>
    <p>Created an AR product demo for a tech company that enhanced customer interaction and increased lead generation by 25%.</p>
  </div>
</section>

<section id="contact">
  <h2>Contact Me</h2>
  <form class="contact-form" onsubmit="event.preventDefault(); alert('Thank you for reaching out! I will get back to you soon.');">
    <label for="name">Name</label>
    <input type="text" id="name" placeholder="Your name" required />
    <label for="email">Email</label>
    <input type="email" id="email" placeholder="example@mail.com" required />
    <label for="message">Message</label>
    <textarea id="message" rows="4" placeholder="Write your message here..." required></textarea>
    <button type="submit">Send Message</button>
  </form>
</section>

<footer>
  &copy; 2025 Future of Digital Marketing Portfolio
</footer>

<script>
  const tabButtons = document.querySelectorAll('.tab-btn');
  const sections = document.querySelectorAll('section');

  tabButtons.forEach(btn => {
    btn.addEventListener('click', () => {
      tabButtons.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      const target = btn.getAttribute('data-tab');
      sections.forEach(sec => {
        if (sec.id === target) {
          sec.classList.add('active');
        } else {
          sec.classList.remove('active');
        }
      });
    });
  });
</script>

</body>
</html>
