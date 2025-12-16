<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SmartCreatorHub - Grow Smarter with Digital Tools</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&family=Poppins:wght@600;700&display=swap" rel="stylesheet">
<style>
  *{box-sizing:border-box;margin:0;padding:0;}
  body{font-family:'Inter',sans-serif;background:#0D0D0D;color:#FFF;line-height:1.6;overflow-x:hidden;}
  a{text-decoration:none;color:inherit;}
  .container{max-width:1200px;margin:auto;padding:20px;}
  h1,h2,h3{font-family:'Poppins',sans-serif;}

  /* HERO */
  header{text-align:center;padding:100px 20px;background:linear-gradient(135deg,#0D0D0D,#111);position:relative;}
  header h1{font-size:3em;background:linear-gradient(90deg,#00FF85,#00FFA0);-webkit-background-clip:text;-webkit-text-fill-color:transparent;margin-bottom:20px;animation:fadeIn 2s ease-in-out;}
  header p{font-size:1.3em;margin-bottom:30px;animation:fadeIn 2.5s ease-in-out;}
  .btn{display:inline-block;padding:15px 35px;margin:10px;border-radius:12px;background:linear-gradient(90deg,#00FF85,#00FFA0);color:#0D0D0D;font-weight:bold;transition:0.3s;box-shadow:0 5px 15px rgba(0,255,133,0.3);}
  .btn:hover{transform:translateY(-5px);box-shadow:0 10px 25px rgba(0,255,133,0.5);}

  /* COUNTDOWN */
  .countdown{font-size:1.5em;color:#00FF85;margin-top:20px;}

  /* SECTIONS */
  section{padding:60px 20px;text-align:center;}
  section h2{font-size:2.2em;margin-bottom:20px;color:#00FF85;opacity:0;transform:translateY(20px);transition:all 0.8s ease;}
  section p{font-size:1.1em;max-width:700px;margin:auto;margin-bottom:30px;opacity:0;transform:translateY(20px);transition:all 0.8s ease;}
  .reveal{opacity:1!important;transform:translateY(0)!important;}

  /* PRODUCTS */
  .products{display:flex;flex-wrap:wrap;justify-content:center;gap:25px;}
  .product-card{background:#1A1A1A;padding:25px;border-radius:18px;width:300px;transition:all 0.6s ease;transform:translateY(30px);opacity:0;}
  .product-card h3{margin-bottom:15px;color:#00FF85;}
  .product-card p{font-size:1em;margin-bottom:20px;}
  .product-card.reveal{transform:translateY(0);opacity:1;}

  /* SOCIAL PROOF */
  .testimonials{display:flex;flex-wrap:wrap;justify-content:center;gap:20px;margin-top:40px;}
  .testimonial-card{background:#1A1A1A;padding:20px;border-radius:15px;width:250px;opacity:0;transform:translateY(20px);transition:all 0.6s ease;}
  .testimonial-card.reveal{opacity:1;transform:translateY(0);}
  .testimonial-card p{font-size:0.95em;margin-bottom:10px;}
  .testimonial-card h4{font-size:1em;color:#00FF85;}

  /* FOOTER */
  footer{text-align:center;padding:35px 20px;background:#111;font-size:0.9em;color:#AAA;}

  /* POPUP */
  .popup{display:none;position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.85);justify-content:center;align-items:center;z-index:9999;}
  .popup-content{background:#111;padding:30px;border-radius:15px;max-width:400px;text-align:center;}
  .popup-content input{width:80%;padding:10px;margin:10px 0;border-radius:10px;border:none;}
  .popup-content button{padding:12px 25px;border:none;border-radius:10px;background:#00FF85;color:#0D0D0D;font-weight:bold;cursor:pointer;transition:0.3s;}
  .popup-content button:hover{background:#00FFA0;}

  /* STICKY CTA */
  .sticky-cta{position:fixed;bottom:20px;right:20px;background:#00FF85;color:#0D0D0D;padding:15px 25px;border-radius:12px;font-weight:bold;box-shadow:0 5px 15px rgba(0,255,133,0.4);cursor:pointer;transition:0.3s;z-index:999;}
  .sticky-cta:hover{transform:translateY(-5px);box-shadow:0 10px 25px rgba(0,255,133,0.5);}

  /* RESPONSIVE */
  @media(max-width:768px){.products,.testimonials{flex-direction:column;align-items:center;}header h1{font-size:2.5em;}}

  /* ANIMATIONS */
  @keyframes fadeIn{0%{opacity:0;transform:translateY(20px);}100%{opacity:1;transform:translateY(0);}}

  /* CONFETTI CANVAS */
  #confetti-canvas{position:fixed;top:0;left:0;width:100%;height:100%;pointer-events:none;z-index:9999;}
</style>
</head>
<body>

<!-- HERO -->
<header>
  <h1>SmartCreatorHub</h1>
  <p>Grow Smarter with Ready-to-Use Digital Tools.<br>Canva Templates & AI Prompts for Creators, Coaches & Small Brands.</p>
  <div class="countdown" id="countdown"></div>
  <a href="https://obs13.gumroad.com/l/bzfprn" class="btn" target="_blank">Shop Now</a>
  <a href="https://obs13.gumroad.com/l/bzfprn" class="btn" target="_blank">Get Free Template</a>
</header>

<!-- BENEFITS -->
<section>
  <h2 class="reveal">Why Choose SmartCreatorHub?</h2>
  <p class="reveal">Save hours of work, no design or AI skills required, instant digital downloads, lifetime access. Everything you need to grow smarter as a creator.</p>
</section>

<!-- PRODUCTS -->
<section id="products">
  <h2 class="reveal">Our Products</h2>
  <div class="products">
    <div class="product-card">
      <h3>Creator Growth Canva Pack</h3>
      <p>100+ editable templates for Instagram Carousels, Reels, Stories & Hooks.</p>
      <a href="https://obs13.gumroad.com/l/bzfprn" class="btn" target="_blank">Buy Now – $29</a>
    </div>
    <div class="product-card">
      <h3>AI Content Machine Prompts</h3>
      <p>100+ ChatGPT prompts for viral hooks, captions, carousels & content planning.</p>
      <a href="https://obs13.gumroad.com/l/bzfprn" class="btn" target="_blank">Buy Now – $19</a>
    </div>
    <div class="product-card">
      <h3>Creator Combo Bundle</h3>
      <p>Everything in one bundle – Templates + AI Prompts to save hours every week.</p>
      <a href="https://obs13.gumroad.com/l/bzfprn" class="btn" target="_blank">Buy & Save – $39</a>
    </div>
  </div>
</section>

<!-- FREEBIE -->
<section id="freebie">
  <h2 class="reveal">Grab Your Free Creator Starter Pack</h2>
  <p class="reveal">1 Canva template + 5 AI prompts to start creating smarter today!</p>
  <a href="https://obs13.gumroad.com/l/bzfprn" class="btn" target="_blank">Get Free Template</a>
</section>

<!-- SOCIAL PROOF -->
<section>
  <h2 class="reveal">What Our Creators Say</h2>
  <div class="testimonials">
    <div class="testimonial-card">
      <p>"SmartCreatorHub saved me hours every week! Templates are amazing."</p>
      <h4>- Jane D.</h4>
    </div>
    <div class="testimonial-card">
      <p>"The AI prompts are a game changer for content planning."</p>
      <h4>- Mark T.</h4>
    </div>
    <div class="testimonial-card">
      <p>"Loved the combo bundle! Best investment for creators."</p>
      <h4>- Sarah K.</h4>
    </div>
  </div>
</section>

<!-- FINAL CTA -->
<section>
  <h2 class="reveal">Create Smarter. Grow Faster.</h2>
  <a href="https://obs13.gumroad.com/l/bzfprn" class="btn" target="_blank">Start Now</a>
</section>

<!-- FOOTER -->
<footer>
  <p>© 2025 SmartCreatorHub | <a href="https://smartcreatorhub.com" style="color:#00FF85;">smartcreatorhub.com</a></p>
</footer>

<!-- EMAIL POPUP -->
<div class="popup" id="popup">
  <div class="popup-content">
    <h3>Join Our Creator Community!</h3>
    <p>Get free templates & AI prompts in your inbox</p>
    <form action="https://app.lastapp.ai/share/b96b2b48-882e-44d5-89b7-994969a63e43" method="post" target="_blank">
      <input type="email" placeholder="Enter your email" name="EMAIL" required>
      <button type="submit" id="subscribeBtn">Subscribe</button>
    </form>
  </div>
</div>

<!-- STICKY CTA -->
<div class="sticky-cta" onclick="window.open('https://obs13.gumroad.com/l/bzfprn','_blank')">Get Started</div>

<!-- CONFETTI CANVAS -->
<canvas id="confetti-canvas"></canvas>

<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
<script>
  // SCROLL REVEAL
  const revealElements = document.querySelectorAll('.reveal, .product-card, .testimonial-card');
  function reveal() {
    const windowHeight = window.innerHeight;
    revealElements.forEach(el => {
      const elementTop = el.getBoundingClientRect().top;
      if(elementTop < windowHeight - 100){ el.classList.add('reveal'); }
    });
  }
  window.addEventListener('scroll', reveal);
  window.addEventListener('load', reveal);

  // COUNTDOWN TIMER
  const countdown = document.getElementById('countdown');
  const countDownDate = new Date("Mar 16, 2026 23:59:00").getTime();
  setInterval(() => {
    const now = new Date().getTime();
    const distance = countDownDate - now;
    const days = Math.floor(distance / (1000*60*60*24));
    const hours = Math.floor((distance % (1000*60*60*24)) / (1000*60*60));
    const minutes = Math.floor((distance % (1000*60*60)) / (1000*60));
    const seconds = Math.floor((distance % (1000*60)) / 1000);
    countdown.innerHTML = `Offer ends in ${days}d ${hours}h ${minutes}m ${seconds}s`;
    if(distance < 0){ countdown.innerHTML = "Offer has ended"; }
  }, 1000);

  // EMAIL POPUP
  const popup = document.getElementById('popup');
  setTimeout(()=>{ popup.style.display='flex'; },3000);

  // CONFETTI ON SUBSCRIBE
  document.getElementById('subscribeBtn').addEventListener('click', ()=>{
    setTimeout(()=>{ 
      confetti({
        particleCount:150,
        spread:60,
        origin:{y:0.6}
      });
    },500);
  });
</script>
</body>
</html>