<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Djhona Longrich Internationale – Santé, Beauté & Liberté Financière</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Nunito:wght@300;400;600;700;800&display=swap" rel="stylesheet">
<style>
:root {
  --gold: #C9A84C;
  --gold-light: #F0D080;
  --dark: #0A0E1A;
  --dark2: #12182B;
  --green: #1DB954;
  --green2: #0f9c42;
  --white: #F9F5EC;
  --accent: #E8F5E9;
}

* { margin: 0; padding: 0; box-sizing: border-box; }

html { scroll-behavior: smooth; }

body {
  font-family: 'Nunito', sans-serif;
  background: var(--dark);
  color: var(--white);
  overflow-x: hidden;
}

/* ===== NAVBAR ===== */
nav {
  position: fixed; top: 0; width: 100%; z-index: 999;
  background: rgba(10,14,26,0.92);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(201,168,76,0.25);
  display: flex; justify-content: space-between; align-items: center;
  padding: 14px 5%;
}
.logo {
  font-family: 'Playfair Display', serif;
  font-size: 1.3rem; color: var(--gold);
  letter-spacing: 1px;
}
.logo span { color: var(--green); }
.nav-links { display: flex; gap: 28px; list-style: none; }
.nav-links a {
  color: var(--white); text-decoration: none;
  font-size: 0.9rem; font-weight: 600;
  transition: color 0.3s;
  letter-spacing: 0.5px;
}
.nav-links a:hover { color: var(--gold); }
.nav-cta {
  background: linear-gradient(135deg, var(--gold), var(--gold-light));
  color: var(--dark) !important;
  padding: 8px 22px; border-radius: 30px;
  font-weight: 800 !important;
}

/* ===== HERO ===== */
.hero {
  min-height: 100vh;
  background: radial-gradient(ellipse at 30% 60%, rgba(29,185,84,0.12) 0%, transparent 60%),
              radial-gradient(ellipse at 80% 20%, rgba(201,168,76,0.15) 0%, transparent 55%),
              linear-gradient(180deg, #0A0E1A 0%, #0d1420 100%);
  display: flex; align-items: center;
  padding: 100px 5% 60px;
  position: relative; overflow: hidden;
}
.hero::before {
  content: '';
  position: absolute; top: -50%; left: -10%;
  width: 70%; height: 200%;
  background: radial-gradient(ellipse, rgba(29,185,84,0.06) 0%, transparent 70%);
  animation: pulse 6s ease-in-out infinite;
}
@keyframes pulse {
  0%,100% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.05); opacity: 0.7; }
}

.hero-content { max-width: 620px; z-index: 1; }
.hero-badge {
  display: inline-block;
  background: rgba(29,185,84,0.15);
  border: 1px solid var(--green);
  color: var(--green); font-size: 0.82rem; font-weight: 700;
  padding: 6px 18px; border-radius: 30px; margin-bottom: 24px;
  letter-spacing: 1px; text-transform: uppercase;
  animation: fadeInDown 0.8s ease;
}
.hero h1 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2.4rem, 5vw, 4rem);
  line-height: 1.15;
  margin-bottom: 20px;
  animation: fadeInUp 0.9s ease 0.1s both;
}
.hero h1 .highlight {
  background: linear-gradient(135deg, var(--gold), var(--gold-light));
  -webkit-background-clip: text; -webkit-text-fill-color: transparent;
  background-clip: text;
}
.hero p {
  font-size: 1.1rem; color: rgba(249,245,236,0.75);
  line-height: 1.7; margin-bottom: 36px;
  animation: fadeInUp 0.9s ease 0.2s both;
}
.hero-btns {
  display: flex; gap: 16px; flex-wrap: wrap;
  animation: fadeInUp 0.9s ease 0.3s both;
}
.btn-gold {
  background: linear-gradient(135deg, var(--gold), var(--gold-light));
  color: var(--dark); padding: 14px 32px; border-radius: 50px;
  font-weight: 800; font-size: 1rem; text-decoration: none;
  transition: transform 0.3s, box-shadow 0.3s;
  display: inline-flex; align-items: center; gap: 8px;
}
.btn-gold:hover { transform: translateY(-3px); box-shadow: 0 12px 40px rgba(201,168,76,0.4); }
.btn-outline {
  border: 2px solid var(--green); color: var(--green);
  padding: 14px 32px; border-radius: 50px;
  font-weight: 800; font-size: 1rem; text-decoration: none;
  transition: all 0.3s; display: inline-flex; align-items: center; gap: 8px;
}
.btn-outline:hover { background: var(--green); color: white; transform: translateY(-3px); }

.hero-stats {
  display: flex; gap: 40px; margin-top: 50px;
  animation: fadeInUp 0.9s ease 0.4s both;
}
.stat { text-align: center; }
.stat-num {
  font-family: 'Playfair Display', serif;
  font-size: 2rem; color: var(--gold); font-weight: 900;
}
.stat-label { font-size: 0.8rem; color: rgba(249,245,236,0.6); text-transform: uppercase; letter-spacing: 1px; }

.hero-visual {
  position: absolute; right: 3%; top: 50%;
  transform: translateY(-50%);
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 12px; width: 380px;
  animation: fadeInRight 1s ease 0.3s both;
}
.hero-img-card {
  border-radius: 16px; overflow: hidden;
  box-shadow: 0 8px 30px rgba(0,0,0,0.5);
  border: 1px solid rgba(201,168,76,0.2);
  aspect-ratio: 1;
  background: var(--dark2);
  display: flex; align-items: center; justify-content: center;
  position: relative;
}
.hero-img-card img { width: 100%; height: 100%; object-fit: cover; }
.hero-img-card:first-child { grid-column: span 2; aspect-ratio: 2/1; }

@keyframes fadeInDown { from { opacity:0; transform:translateY(-20px);} to {opacity:1; transform:translateY(0);} }
@keyframes fadeInUp { from { opacity:0; transform:translateY(30px);} to {opacity:1; transform:translateY(0);} }
@keyframes fadeInRight { from { opacity:0; transform:translateX(40px) translateY(-50%);} to {opacity:1; transform:translateX(0) translateY(-50%);} }

/* ===== SECTION TITLES ===== */
.section { padding: 90px 5%; }
.section-header { text-align: center; margin-bottom: 60px; }
.section-tag {
  display: inline-block; font-size: 0.78rem;
  font-weight: 700; letter-spacing: 2px; text-transform: uppercase;
  color: var(--green); margin-bottom: 12px;
}
.section-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2rem, 4vw, 3rem);
  line-height: 1.2;
}
.section-title span {
  background: linear-gradient(135deg, var(--gold), var(--gold-light));
  -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
}
.section-sub {
  color: rgba(249,245,236,0.65); font-size: 1.05rem;
  max-width: 580px; margin: 14px auto 0; line-height: 1.7;
}

/* ===== TICKER BANNER ===== */
.ticker {
  background: linear-gradient(135deg, var(--gold), var(--gold-light));
  overflow: hidden; padding: 14px 0; white-space: nowrap;
}
.ticker-inner {
  display: inline-block;
  animation: ticker 25s linear infinite;
}
.ticker-item {
  display: inline-block; color: var(--dark);
  font-weight: 800; font-size: 0.9rem;
  padding: 0 40px; letter-spacing: 0.5px;
}
.ticker-item::before { content: '✦ '; }
@keyframes ticker { from { transform: translateX(0); } to { transform: translateX(-50%); } }

/* ===== PRODUCTS ===== */
.products-bg {
  background: linear-gradient(180deg, var(--dark) 0%, var(--dark2) 50%, var(--dark) 100%);
}
.products-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 24px;
}
.product-card {
  background: rgba(255,255,255,0.04);
  border: 1px solid rgba(201,168,76,0.15);
  border-radius: 20px; overflow: hidden;
  transition: transform 0.35s, box-shadow 0.35s, border-color 0.35s;
  cursor: pointer;
  position: relative;
}
.product-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 20px 50px rgba(201,168,76,0.2);
  border-color: rgba(201,168,76,0.5);
}
.product-img {
  width: 100%; aspect-ratio: 4/3;
  object-fit: cover; display: block;
  background: var(--dark2);
}
.product-badge {
  position: absolute; top: 14px; left: 14px;
  background: var(--green); color: white;
  font-size: 0.72rem; font-weight: 800;
  padding: 4px 12px; border-radius: 20px;
  text-transform: uppercase; letter-spacing: 0.5px;
}
.product-info { padding: 20px; }
.product-category {
  font-size: 0.72rem; font-weight: 700; color: var(--gold);
  text-transform: uppercase; letter-spacing: 1.5px; margin-bottom: 6px;
}
.product-name {
  font-family: 'Playfair Display', serif;
  font-size: 1.25rem; margin-bottom: 8px;
}
.product-desc {
  font-size: 0.88rem; color: rgba(249,245,236,0.6);
  line-height: 1.6; margin-bottom: 18px;
}
.product-footer { display: flex; justify-content: space-between; align-items: center; }
.product-stars { color: var(--gold); font-size: 0.9rem; }
.btn-buy {
  background: linear-gradient(135deg, #25D366, #128C7E);
  color: white; padding: 8px 20px; border-radius: 30px;
  font-weight: 700; font-size: 0.85rem; text-decoration: none;
  transition: all 0.3s; display: flex; align-items: center; gap: 6px;
}
.btn-buy:hover { transform: scale(1.05); box-shadow: 0 6px 20px rgba(37,211,102,0.4); }

/* ===== BENEFITS ===== */
.benefits-grid {
  display: grid; grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
  gap: 28px;
}
.benefit-card {
  background: rgba(29,185,84,0.06);
  border: 1px solid rgba(29,185,84,0.2);
  border-radius: 20px; padding: 32px 26px;
  text-align: center;
  transition: transform 0.3s, border-color 0.3s;
}
.benefit-card:hover { transform: translateY(-6px); border-color: var(--green); }
.benefit-icon { font-size: 2.8rem; margin-bottom: 18px; }
.benefit-title { font-family: 'Playfair Display', serif; font-size: 1.2rem; margin-bottom: 10px; }
.benefit-desc { font-size: 0.9rem; color: rgba(249,245,236,0.65); line-height: 1.6; }

/* ===== TESTIMONIALS ===== */
.testimonials-bg {
  background: radial-gradient(ellipse at center, rgba(201,168,76,0.07) 0%, transparent 70%),
              linear-gradient(180deg, var(--dark2) 0%, var(--dark) 100%);
}
.testimonials-grid {
  display: grid; grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 24px;
}
.testi-card {
  background: rgba(255,255,255,0.04);
  border: 1px solid rgba(201,168,76,0.2);
  border-radius: 20px; padding: 30px;
  position: relative; transition: transform 0.3s;
}
.testi-card:hover { transform: translateY(-5px); }
.testi-card::before {
  content: '"';
  position: absolute; top: -10px; left: 20px;
  font-family: 'Playfair Display', serif;
  font-size: 6rem; color: var(--gold); opacity: 0.2;
  line-height: 1;
}
.testi-stars { color: var(--gold); font-size: 1rem; margin-bottom: 14px; }
.testi-text {
  font-size: 0.95rem; line-height: 1.7;
  color: rgba(249,245,236,0.82); margin-bottom: 22px;
  font-style: italic;
}
.testi-author { display: flex; align-items: center; gap: 14px; }
.testi-avatar {
  width: 46px; height: 46px; border-radius: 50%;
  background: linear-gradient(135deg, var(--gold), var(--green));
  display: flex; align-items: center; justify-content: center;
  font-weight: 800; font-size: 1.1rem; color: var(--dark);
  flex-shrink: 0;
}
.testi-name { font-weight: 700; font-size: 0.95rem; }
.testi-role { font-size: 0.78rem; color: var(--gold); }

/* ===== INCOME PROOF BANNER ===== */
.income-banner {
  background: linear-gradient(135deg, rgba(29,185,84,0.15), rgba(201,168,76,0.1));
  border: 1px solid rgba(201,168,76,0.3);
  border-radius: 30px; padding: 60px 5%;
  text-align: center; margin: 0 5%;
  position: relative; overflow: hidden;
}
.income-banner::before {
  content: '';
  position: absolute; top: -50%; left: -10%;
  width: 120%; height: 200%;
  background: radial-gradient(ellipse, rgba(201,168,76,0.08), transparent 60%);
  animation: pulse 5s ease-in-out infinite;
}
.income-banner h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(1.8rem, 3.5vw, 2.8rem);
  margin-bottom: 16px; position: relative; z-index: 1;
}
.income-banner p {
  font-size: 1.05rem; color: rgba(249,245,236,0.75);
  max-width: 600px; margin: 0 auto 30px; position: relative; z-index: 1; line-height: 1.7;
}
.income-numbers {
  display: flex; justify-content: center; gap: 60px; flex-wrap: wrap;
  position: relative; z-index: 1; margin-bottom: 36px;
}
.income-num {
  font-family: 'Playfair Display', serif;
  font-size: 2.4rem; color: var(--gold); font-weight: 900;
}
.income-label { font-size: 0.82rem; color: rgba(249,245,236,0.6); text-transform: uppercase; letter-spacing: 1px; }

/* ===== PARTNER SECTION ===== */
.partner-section {
  background: linear-gradient(135deg, #0d1f0f 0%, #0A0E1A 50%, #1a1200 100%);
  position: relative; overflow: hidden;
}
.partner-section::before {
  content: '';
  position: absolute; top: 0; left: 0; width: 100%; height: 100%;
  background: radial-gradient(ellipse at 20% 50%, rgba(29,185,84,0.12) 0%, transparent 60%),
              radial-gradient(ellipse at 80% 50%, rgba(201,168,76,0.1) 0%, transparent 60%);
}
.partner-grid {
  display: grid; grid-template-columns: 1fr 1fr; gap: 60px; align-items: center;
  position: relative; z-index: 1;
}
.partner-content h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2rem, 3.5vw, 2.8rem); margin-bottom: 20px;
}
.partner-content p {
  font-size: 1rem; line-height: 1.8; color: rgba(249,245,236,0.75); margin-bottom: 30px;
}
.partner-steps { display: flex; flex-direction: column; gap: 20px; }
.step {
  display: flex; gap: 18px; align-items: flex-start;
}
.step-num {
  width: 42px; height: 42px; border-radius: 50%;
  background: linear-gradient(135deg, var(--gold), var(--gold-light));
  color: var(--dark); font-weight: 900; font-size: 1rem;
  display: flex; align-items: center; justify-content: center;
  flex-shrink: 0; margin-top: 2px;
}
.step-text h4 { font-size: 1rem; font-weight: 700; margin-bottom: 4px; }
.step-text p { font-size: 0.88rem; color: rgba(249,245,236,0.65); line-height: 1.5; }

.partner-card {
  background: rgba(255,255,255,0.04);
  border: 1px solid rgba(201,168,76,0.25);
  border-radius: 28px; padding: 44px 36px;
  text-align: center;
}
.partner-card h3 {
  font-family: 'Playfair Display', serif;
  font-size: 1.7rem; margin-bottom: 14px;
}
.partner-card > p { font-size: 0.95rem; color: rgba(249,245,236,0.7); margin-bottom: 30px; line-height: 1.6; }
.partner-perks { display: flex; flex-direction: column; gap: 12px; margin-bottom: 36px; text-align: left; }
.perk {
  display: flex; align-items: center; gap: 12px;
  font-size: 0.92rem; color: rgba(249,245,236,0.85);
}
.perk-icon { color: var(--green); font-size: 1.1rem; flex-shrink: 0; }

/* ===== WHATSAPP FLOAT ===== */
.wa-float {
  position: fixed; bottom: 30px; right: 30px; z-index: 1000;
}
.wa-btn {
  width: 62px; height: 62px; border-radius: 50%;
  background: linear-gradient(135deg, #25D366, #128C7E);
  display: flex; align-items: center; justify-content: center;
  font-size: 1.8rem; text-decoration: none; color: white;
  box-shadow: 0 6px 30px rgba(37,211,102,0.5);
  animation: wa-pulse 2s ease-in-out infinite;
}
@keyframes wa-pulse {
  0%,100% { box-shadow: 0 6px 30px rgba(37,211,102,0.5); }
  50% { box-shadow: 0 6px 50px rgba(37,211,102,0.8); transform: scale(1.05); }
}

/* ===== FOOTER ===== */
footer {
  background: #060810;
  border-top: 1px solid rgba(201,168,76,0.2);
  padding: 50px 5% 30px;
}
.footer-grid { display: grid; grid-template-columns: 2fr 1fr 1fr; gap: 40px; margin-bottom: 40px; }
.footer-brand .logo { font-size: 1.5rem; display: block; margin-bottom: 14px; }
.footer-brand p { font-size: 0.9rem; color: rgba(249,245,236,0.55); line-height: 1.7; max-width: 300px; }
.footer-col h4 { color: var(--gold); font-size: 0.85rem; text-transform: uppercase; letter-spacing: 1.5px; margin-bottom: 16px; }
.footer-col ul { list-style: none; display: flex; flex-direction: column; gap: 10px; }
.footer-col ul li a { color: rgba(249,245,236,0.6); text-decoration: none; font-size: 0.9rem; transition: color 0.3s; }
.footer-col ul li a:hover { color: var(--gold); }
.footer-bottom {
  border-top: 1px solid rgba(201,168,76,0.1);
  padding-top: 24px; text-align: center;
  font-size: 0.82rem; color: rgba(249,245,236,0.4);
}

/* ===== RESPONSIVE ===== */
@media (max-width: 900px) {
  .hero-visual { display: none; }
  .hero { text-align: center; }
  .hero-btns { justify-content: center; }
  .hero-stats { justify-content: center; }
  .partner-grid { grid-template-columns: 1fr; }
  .footer-grid { grid-template-columns: 1fr 1fr; }
  nav .nav-links { display: none; }
}
@media (max-width: 600px) {
  .footer-grid { grid-template-columns: 1fr; }
  .income-numbers { gap: 30px; }
}

/* ===== DIVIDER ===== */
.gold-divider {
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
  margin: 0 5%;
}

/* ===== URGENCY BAR ===== */
.urgency-bar {
  background: linear-gradient(135deg, #8B0000, #C0392B);
  text-align: center; padding: 10px;
  font-size: 0.88rem; font-weight: 700; letter-spacing: 0.5px;
}
.urgency-bar span { color: var(--gold-light); }
</style>
</head>
<body>

<!-- URGENCY BAR -->
<div class="urgency-bar">
  🔥 <span>OFFRE LIMITÉE :</span> Commandez aujourd'hui via WhatsApp et recevez un BONUS surprise ! +22657995415
</div>

<!-- NAV -->
<nav>
  <div class="logo">Djhona <span>Longrich</span> Int.</div>
  <ul class="nav-links">
    <li><a href="#produits">Produits</a></li>
    <li><a href="#temoignages">Témoignages</a></li>
    <li><a href="#partenaire">Devenir Partenaire</a></li>
    <li><a href="#contact" class="nav-cta">Commander</a></li>
  </ul>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-content">
    <div class="hero-badge">✦ Marque Mondiale de Confiance</div>
    <h1>
      Santé, Beauté &<br>
      <span class="highlight">Liberté Financière</span><br>
      avec Longrich
    </h1>
    <p>
      Des produits naturels de haute qualité qui transforment votre vie — et une opportunité unique de générer des revenus illimités depuis chez vous. <strong>Plus de 50 000 familles</strong> en ont déjà bénéficié en Afrique !
    </p>
    <div class="hero-btns">
      <a href="https://wa.me/22657995415" target="_blank" class="btn-gold">
        🛒 Commander Maintenant
      </a>
      <a href="#partenaire" class="btn-outline">
        💰 Devenir Partenaire
      </a>
    </div>
    <div class="hero-stats">
      <div class="stat">
        <div class="stat-num">50K+</div>
        <div class="stat-label">Clients Satisfaits</div>
      </div>
      <div class="stat">
        <div class="stat-num">100%</div>
        <div class="stat-label">Naturel</div>
      </div>
      <div class="stat">
        <div class="stat-num">30+</div>
        <div class="stat-label">Pays</div>
      </div>
    </div>
  </div>

  <div class="hero-visual">
    <div class="hero-img-card">
      <img src="https://via.placeholder.com/400x200/1DB954/FFFFFF?text=Longrich+Products" alt="Longrich Products">
    </div>
    <div class="hero-img-card">
      <img src="https://via.placeholder.com/200x200/C9A84C/FFFFFF?text=Beauté" alt="Beauté">
    </div>
    <div class="hero-img-card">
      <img src="https://via.placeholder.com/200x200/0A0E1A/C9A84C?text=Santé" alt="Santé">
    </div>
  </div>
</section>

<!-- TICKER -->
<div class="ticker">
  <div class="ticker-inner">
    <span class="ticker-item">Livraison rapide</span>
    <span class="ticker-item">Produits 100% naturels</span>
    <span class="ticker-item">Résultats garantis</span>
    <span class="ticker-item">Des milliers de clients satisfaits</span>
    <span class="ticker-item">Rejoignez la famille Longrich</span>
    <span class="ticker-item">Gagnez de l'argent chez vous</span>
    <span class="ticker-item">Qualité certifiée internationale</span>
    <span class="ticker-item">Livraison rapide</span>
    <span class="ticker-item">Produits 100% naturels</span>
    <span class="ticker-item">Résultats garantis</span>
    <span class="ticker-item">Des milliers de clients satisfaits</span>
    <span class="ticker-item">Rejoignez la famille Longrich</span>
    <span class="ticker-item">Gagnez de l'argent chez vous</span>
    <span class="ticker-item">Qualité certifiée internationale</span>
  </div>
</div>

<!-- PRODUCTS -->
<section class="section products-bg" id="produits">
  <div class="section-header">
    <div class="section-tag">Nos Produits Phares</div>
    <h2 class="section-title">Des produits qui <span>changent des vies</span></h2>
    <p class="section-sub">Chaque produit Longrich est fo
