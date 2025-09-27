<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>NR Vision Tech | IT Solutions & Staffing</title>
  <style>
    :root {
      --primary: #1a237e;
      --secondary: #3949ab;
      --accent: #90caf9;
      --text: #333;
      --bg: #f9fafc;
    }
    * {
      box-sizing: border-box;
      scroll-behavior: smooth;
    }
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    /* Header */
    header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: #ffffff; /* Light header to match bright image */
      color: #333;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      border-bottom: 1px solid #e0e0e0;
      transition: box-shadow 0.3s ease;
    }
    header.scrolled {
      box-shadow: 0 3px 8px rgba(0,0,0,0.1);
    }
    header h1 {
      margin: 0;
      font-size: 1.8rem;
      font-weight: 600;
      color: var(--primary);
    }
    nav a {
      margin: 0 14px;
      color: var(--primary);
      text-decoration: none;
      font-weight: 600;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: var(--secondary);
    }

    /* Hero */
    .hero {
      background: url('https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&w=1600&q=80')
                  no-repeat center center/cover;
      text-align: center;
      padding: 7rem 1rem;
    }
    .hero h2 {
      font-size: 2.8rem;
      margin-bottom: 1rem;
      color: #ffffff;
      text-shadow: 0 2px 6px rgba(0,0,0,0.5);
      animation: fadeInDown 1s ease-in-out;
    }
    .hero p {
      font-size: 1.2rem;
      max-width: 700px;
      margin: auto;
      color: #ffffff;
      text-shadow: 0 2px 4px rgba(0,0,0,0.4);
      animation: fadeInUp 1.2s ease-in-out;
    }
    .hero .cta-btn {
      display: inline-block;
      margin-top: 2rem;
      padding: 0.8rem 1.8rem;
      background: var(--primary);
      color: #fff;
      font-weight: bold;
      border-radius: 50px;
      text-decoration: none;
      transition: background 0.3s ease;
    }
    .hero .cta-btn:hover {
      background: var(--secondary);
    }

    /* Sections */
    section {
      padding: 4rem 1rem;
      max-width: 1100px;
      margin: auto;
      text-align: center;
    }
    section h2 {
      color: var(--primary);
      font-size: 2rem;
      margin-bottom: 1.5rem;
      position: relative;
    }
    section h2::after {
      content: '';
      display: block;
      width: 60px;
      height: 4px;
      background: var(--accent);
      margin: 0.5rem auto 0;
      border-radius: 2px;
    }
    section p {
      max-width: 800px;
      margin: auto;
      font-size: 1.05rem;
    }

    /* Services */
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1.8rem;
      margin-top: 2.5rem;
    }
    .card {
      background: #fff;
      padding: 2rem 1.5rem;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.08);
      transition: transform 0.25s ease, box-shadow 0.25s ease;
    }
    .card h3 {
      color: var(--secondary);
      margin-bottom: 0.8rem;
    }
    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 8px 18px rgba(0,0,0,0.15);
    }

    /* Footer */
    footer {
      background: #f7f7f7;
      color: #555;
      text-align: center;
      padding: 1.5rem;
      border-top: 1px solid #e0e0e0;
    }
    footer a {
      color: var(--primary);
      text-decoration: none;
    }
    footer a:hover {
      color: var(--secondary);
    }

    /* Animations */
    @keyframes fadeInDown {
      0% {opacity:0;transform:translateY(-20px);}
      100% {opacity:1;transform:translateY(0);}
    }
    @keyframes fadeInUp {
      0% {opacity:0;transform:translateY(20px);}
      100% {opacity:1;transform:translateY(0);}
    }

    /* Responsive */
    @media (max-width: 600px) {
      header {
        flex-direction: column;
        text-align: center;
      }
      nav {
        margin-top: 0.5rem;
      }
      .hero h2 {font-size: 2.2rem;}
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header id="main-header">
    <h1>NR Vision Tech</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#careers">Careers</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero">
    <h2>Empowering Businesses with Technology & Talent</h2>
    <p>Innovative IT solutions and staffing services to help companies thrive in a digital world.</p>
    <a href="#contact" class="cta-btn">Get in Touch</a>
  </section>

  <!-- About -->
  <section id="about">
    <h2>About Us</h2>
    <p>
      <strong>NR Vision Tech</strong> delivers innovative IT solutions and staffing services tailored to the needs of modern businesses. 
      Our mission is to empower organizations with the right technology and people to achieve their vision.
    </p>
  </section>

  <!-- Services -->
  <section id="services">
    <h2>Our Services</h2>
    <div class="services">
      <div class="card">
        <h3>IT Consulting</h3>
        <p>Expert guidance on cloud, cybersecurity, and enterprise IT solutions.</p>
      </div>
      <div class="card">
        <h3>Staffing Solutions</h3>
        <p>Connecting companies with top tech talent for contract and full-time roles.</p>
      </div>
      <div class="card">
        <h3>Custom Software</h3>
        <p>Scalable, secure applications tailored to business requirements.</p>
      </div>
      <div class="card">
        <h3>Managed Services</h3>
        <p>End-to-end IT infrastructure management to reduce downtime and costs.</p>
      </div>
      <div class="card">
        <h3>Training & Placement</h3>
        <p>Upskill and prepare for your ideal career path in technology.</p>
      </div>
    </div>
  </section>

  <!-- Careers -->
  <section id="careers">
    <h2>Careers</h2>
    <p>
      Join our growing team of IT professionals! We’re always looking for passionate
      individuals in software development, cloud engineering, data analytics, and more.
      Send your resume to <a href="mailto:careers@nrvisiontech.com">careers@nrvisiontech.com</a>.
    </p>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact Us</h2>
    <p>
      📧 Email: <a href="mailto:contact@nrvisiontech.com">contact@nrvisiontech.com</a><br>
      📍 Location: Florida, USA<br>
      📞 Phone: +1 (813) 848 9234
    </p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 NR Vision Tech | IT Solutions & Staffing</p>
  </footer>

  <script>
    // Add shadow to header on scroll
    window.addEventListener('scroll', () => {
      const header = document.getElementById('main-header');
      header.classList.toggle('scrolled', window.scrollY > 20);
    });
  </script>
</body>
</html>
