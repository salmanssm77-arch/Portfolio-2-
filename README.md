<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Salman Mangalgiri | Futuristic Portfolio</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      scroll-behavior:smooth;
      font-family:'Poppins',sans-serif;
    }

    body{
      background:#050816;
      color:white;
      overflow-x:hidden;
    }

    body::before{
      content:'';
      position:fixed;
      width:500px;
      height:500px;
      background:radial-gradient(circle,#6d28d9 0%,transparent 70%);
      top:-150px;
      left:-100px;
      opacity:0.4;
      filter:blur(70px);
      z-index:-1;
      animation:float 8s infinite alternate;
    }

    body::after{
      content:'';
      position:fixed;
      width:400px;
      height:400px;
      background:radial-gradient(circle,#2563eb 0%,transparent 70%);
      bottom:-150px;
      right:-100px;
      opacity:0.4;
      filter:blur(70px);
      z-index:-1;
      animation:float 10s infinite alternate;
    }

    @keyframes float{
      from{transform:translateY(0px)}
      to{transform:translateY(40px)}
    }

    nav{
      position:fixed;
      top:0;
      width:100%;
      padding:20px 10%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      background:rgba(255,255,255,0.05);
      backdrop-filter:blur(15px);
      border-bottom:1px solid rgba(255,255,255,0.1);
      z-index:1000;
    }

    nav h1{
      font-size:28px;
      background:linear-gradient(to right,#60a5fa,#c084fc);
      -webkit-background-clip:text;
      color:transparent;
      font-weight:800;
    }

    nav ul{
      display:flex;
      gap:30px;
      list-style:none;
    }

    nav ul li a{
      color:white;
      text-decoration:none;
      transition:0.3s;
      font-weight:500;
    }

    nav ul li a:hover{
      color:#a855f7;
    }

    section{
      padding:120px 10%;
    }

    .hero{
      min-height:100vh;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:50px;
      flex-wrap:wrap;
    }

    .hero-text{
      flex:1;
    }

    .hero-text h2{
      font-size:70px;
      line-height:1.1;
      margin-bottom:20px;
      background:linear-gradient(to right,#ffffff,#a855f7,#60a5fa);
      -webkit-background-clip:text;
      color:transparent;
    }

    .typing{
      font-size:24px;
      color:#c084fc;
      margin-bottom:25px;
      min-height:40px;
    }

    .hero-text p{
      color:#cbd5e1;
      line-height:1.8;
      max-width:650px;
      margin-bottom:30px;
    }

    .btns{
      display:flex;
      gap:20px;
      flex-wrap:wrap;
    }

    .btn{
      padding:14px 28px;
      border-radius:50px;
      border:none;
      background:linear-gradient(to right,#7c3aed,#2563eb);
      color:white;
      font-weight:600;
      text-decoration:none;
      transition:0.4s;
      box-shadow:0 0 25px rgba(168,85,247,0.4);
    }

    .btn:hover{
      transform:translateY(-5px) scale(1.05);
      box-shadow:0 0 40px rgba(168,85,247,0.7);
    }

    .hero-image{
      flex:1;
      display:flex;
      justify-content:center;
    }

    .hero-image img{
      width:350px;
      height:350px;
      border-radius:30px;
      object-fit:cover;
      border:2px solid rgba(255,255,255,0.2);
      box-shadow:0 0 40px rgba(168,85,247,0.5);
      animation:float 5s infinite alternate;
    }

    .glass-card{
      background:rgba(255,255,255,0.06);
      border:1px solid rgba(255,255,255,0.1);
      backdrop-filter:blur(20px);
      border-radius:25px;
      padding:30px;
      transition:0.4s;
    }

    .glass-card:hover{
      transform:translateY(-10px);
      box-shadow:0 0 35px rgba(168,85,247,0.35);
    }

    .title{
      font-size:42px;
      margin-bottom:50px;
      text-align:center;
      background:linear-gradient(to right,#60a5fa,#c084fc);
      -webkit-background-clip:text;
      color:transparent;
    }

    .grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:30px;
    }

    .skill h3{
      margin-bottom:15px;
    }

    .bar{
      width:100%;
      height:12px;
      background:#1e293b;
      border-radius:20px;
      overflow:hidden;
    }

    .fill{
      height:100%;
      background:linear-gradient(to right,#7c3aed,#3b82f6);
      border-radius:20px;
    }

    .project img,.certificate img{
      width:100%;
      border-radius:20px;
      margin-bottom:20px;
      border:1px solid rgba(255,255,255,0.1);
    }

    .project h3,.certificate h3{
      margin-bottom:10px;
      font-size:24px;
    }

    .project p,.certificate p{
      color:#cbd5e1;
      line-height:1.7;
    }

    .tags{
      margin-top:15px;
      display:flex;
      flex-wrap:wrap;
      gap:10px;
    }

    .tag{
      background:rgba(168,85,247,0.15);
      border:1px solid rgba(168,85,247,0.4);
      padding:8px 14px;
      border-radius:50px;
      font-size:14px;
    }

    .stats{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:25px;
      margin-top:40px;
    }

    .stat{
      text-align:center;
    }

    .stat h2{
      font-size:55px;
      color:#a855f7;
    }

    .contact-form{
      display:flex;
      flex-direction:column;
      gap:20px;
      max-width:700px;
      margin:auto;
    }

    .contact-form input,
    .contact-form textarea{
      padding:18px;
      border:none;
      border-radius:18px;
      background:rgba(255,255,255,0.08);
      color:white;
      outline:none;
      border:1px solid rgba(255,255,255,0.08);
    }

    footer{
      text-align:center;
      padding:40px 20px;
      color:#94a3b8;
      border-top:1px solid rgba(255,255,255,0.08);
    }

    .socials{
      display:flex;
      gap:20px;
      margin-top:20px;
    }

    .socials a{
      width:50px;
      height:50px;
      display:flex;
      align-items:center;
      justify-content:center;
      border-radius:50%;
      background:rgba(255,255,255,0.08);
      color:white;
      text-decoration:none;
      transition:0.4s;
      font-size:20px;
    }

    .socials a:hover{
      background:#7c3aed;
      transform:translateY(-5px);
      box-shadow:0 0 25px rgba(168,85,247,0.6);
    }

    @media(max-width:900px){
      .hero{
        flex-direction:column-reverse;
        text-align:center;
      }

      .hero-text h2{
        font-size:52px;
      }

      nav ul{
        display:none;
      }

      .btns{
        justify-content:center;
      }

      .socials{
        justify-content:center;
      }
    }
  </style></head>
<body>  <nav>
    <h1>SM.</h1>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#certifications">Certificates</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>  <section class="hero">
    <div class="hero-text">
      <h2>Salman Mangalgiri</h2>
      <div class="typing"></div>
      <p>
        BBA in Fintech student passionate about finance, AI, technology, fitness, analytics, and futuristic innovation. Building skills in fintech, web development, AI tools, and data analytics while preparing for CFA and future MBA goals.
      </p><div class="btns">
    <a href="#projects" class="btn">View Projects</a>
    <a href="#contact" class="btn">Contact Me</a>
  </div>

  <div class="socials">
    <a href="#">★</a>
    <a href="#">✦</a>
    <a href="#">✧</a>
  </div>
</div>

<div class="hero-image">
  <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1200&auto=format&fit=crop" alt="Profile Image">
</div>

  </section>  <section id="about">
    <h1 class="title">About Me</h1><div class="glass-card">
  <p style="line-height:2;color:#cbd5e1;font-size:18px;">
    I am Salman Mangalgiri, a passionate BBA in Fintech student at MIT World Peace University Solapur. I am deeply interested in finance, AI, analytics, and futuristic technologies. My goal is to combine business and technology to build innovative fintech solutions and create a strong future in the finance and tech industry.
  </p>

  <div class="stats">
    <div class="glass-card stat">
      <h2>10+</h2>
      <p>Projects & Ideas</p>
    </div>

    <div class="glass-card stat">
      <h2>2+</h2>
      <p>Certifications</p>
    </div>

    <div class="glass-card stat">
      <h2>100%</h2>
      <p>Discipline & Growth</p>
    </div>
  </div>
</div>

  </section>  <section id="skills">
    <h1 class="title">Skills</h1><div class="grid">

  <div class="glass-card skill">
    <h3>HTML</h3>
    <div class="bar"><div class="fill" style="width:90%"></div></div>
  </div>

  <div class="glass-card skill">
    <h3>CSS</h3>
    <div class="bar"><div class="fill" style="width:88%"></div></div>
  </div>

  <div class="glass-card skill">
    <h3>JavaScript</h3>
    <div class="bar"><div class="fill" style="width:75%"></div></div>
  </div>

  <div class="glass-card skill">
    <h3>Finance & Fintech</h3>
    <div class="bar"><div class="fill" style="width:85%"></div></div>
  </div>

  <div class="glass-card skill">
    <h3>AI Tools</h3>
    <div class="bar"><div class="fill" style="width:80%"></div></div>
  </div>

  <div class="glass-card skill">
    <h3>Data Analytics</h3>
    <div class="bar"><div class="fill" style="width:72%"></div></div>
  </div>

</div>

  </section>  <section id="projects">
    <h1 class="title">Projects</h1><div class="grid">

  <div class="glass-card project">
    <img src="https://images.unsplash.com/photo-1517836357463-d25dfeac3438?q=80&w=1200&auto=format&fit=crop">
    <h3>AI Diet & Nutrition Planner</h3>
    <p>AI-powered nutrition and meal planning platform with modern UI and fitness analytics.</p>
    <div class="tags">
      <span class="tag">AI</span>
      <span class="tag">Fitness</span>
      <span class="tag">Analytics</span>
    </div>
  </div>

  <div class="glass-card project">
    <img src="https://images.unsplash.com/photo-1556740749-887f6717d7e4?q=80&w=1200&auto=format&fit=crop">
    <h3>Calorie Burn Predictor</h3>
    <p>Machine learning inspired calorie expenditure prediction project using fitness datasets.</p>
    <div class="tags">
      <span class="tag">ML</span>
      <span class="tag">Health</span>
      <span class="tag">Prediction</span>
    </div>
  </div>

  <div class="glass-card project">
    <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?q=80&w=1200&auto=format&fit=crop">
    <h3>Modern Portfolio Website</h3>
    <p>Luxury futuristic portfolio inspired by Apple, AI startups, and modern fintech dashboards.</p>
    <div class="tags">
      <span class="tag">Web Dev</span>
      <span class="tag">UI/UX</span>
      <span class="tag">Design</span>
    </div>
  </div>

</div>

  </section>  <section id="certifications">
    <h1 class="title">Certifications</h1><div class="grid">

  <div class="glass-card certificate">
    <img src="file_00000000902871fab162428814c48aad" alt="Coursera Certificate">
    <h3>Organizational Behavior: How to Manage People</h3>
    <p>Certified by IESE Business School through Coursera.</p>
  </div>

  <div class="glass-card certificate">
    <img src="file_00000000d75071fabfe079862e618044" alt="Cisco Certificate">
    <h3>Introduction to Modern AI</h3>
    <p>Certified by Cisco Networking Academy & MIT Vishwaprayag University.</p>
  </div>

</div>

  </section>  <section id="contact">
    <h1 class="title">Contact Me</h1><form class="contact-form glass-card">
  <input type="text" placeholder="Your Name">
  <input type="email" placeholder="Your Email">
  <textarea rows="6" placeholder="Your Message"></textarea>
  <button class="btn">Send Message</button>
</form>

  </section>  <footer>
    <h2 style="margin-bottom:10px;">Salman Mangalgiri</h2>
    <p>Future CFA Candidate • Fintech Student • AI & Tech Enthusiast</p>
  </footer>  <script>
    const words = [
      'BBA Fintech Student',
      'Future CFA Candidate',
      'Finance & Tech Enthusiast',
      'AI & Analytics Learner',
      'Fitness & Self Growth Focused'
    ];

    let i = 0;
    let j = 0;
    let currentWord = '';
    let isDeleting = false;
    const typing = document.querySelector('.typing');

    function type(){
      currentWord = words[i];

      if(isDeleting){
        typing.textContent = currentWord.substring(0,j--);
      } else {
        typing.textContent = currentWord.substring(0,j++);
      }

      if(!isDeleting && j === currentWord.length){
        isDeleting = true;
        setTimeout(type,1200);
        return;
      }

      if(isDeleting && j === 0){
        isDeleting = false;
        i = (i + 1) % words.length;
      }

      setTimeout(type,isDeleting ? 40 : 80);
    }

    type();
  </script></body>
</html>
