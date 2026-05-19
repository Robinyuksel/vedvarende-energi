# Avanceret Grøn Energi Hjemmeside

```html
<!DOCTYPE html>
<html lang="da">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Future Energy DK</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins', sans-serif;
    background:#071b11;
    color:white;
    overflow-x:hidden;
}

/* NAVBAR */
nav{
    position:fixed;
    width:100%;
    top:0;
    z-index:1000;
    backdrop-filter:blur(10px);
    background:rgba(0,0,0,0.4);
    padding:20px 8%;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

nav h1{
    color:#67ff9b;
    font-size:28px;
}

nav ul{
    display:flex;
    gap:30px;
    list-style:none;
}

nav a{
    text-decoration:none;
    color:white;
    transition:0.3s;
    font-weight:500;
}

nav a:hover{
    color:#67ff9b;
}

/* HERO */
.hero{
    height:100vh;
    background:
    linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.6)),
    url('https://images.unsplash.com/photo-1509391366360-2e959784a276?q=80&w=1600&auto=format&fit=crop');
    background-size:cover;
    background-position:center;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

.hero-content h2{
    font-size:70px;
    margin-bottom:20px;
    animation:fadeIn 1.5s ease;
}

.hero-content p{
    max-width:800px;
    margin:auto;
    font-size:22px;
    opacity:0.9;
    animation:fadeIn 2s ease;
}

.hero-btn{
    margin-top:35px;
    display:inline-block;
    padding:16px 40px;
    background:#67ff9b;
    color:black;
    border-radius:50px;
    text-decoration:none;
    font-weight:bold;
    transition:0.3s;
}

.hero-btn:hover{
    transform:scale(1.1);
    box-shadow:0 0 20px #67ff9b;
}

/* SECTIONS */
section{
    padding:120px 8%;
}

.section-title{
    text-align:center;
    font-size:50px;
    margin-bottom:70px;
    color:#67ff9b;
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
    gap:30px;
}

.card{
    background:rgba(255,255,255,0.05);
    border:1px solid rgba(255,255,255,0.1);
    border-radius:25px;
    overflow:hidden;
    transition:0.4s;
    backdrop-filter:blur(10px);
}

.card:hover{
    transform:translateY(-10px);
    box-shadow:0 10px 35px rgba(103,255,155,0.25);
}

.card img{
    width:100%;
    height:240px;
    object-fit:cover;
}

.card-content{
    padding:25px;
}

.card h3{
    margin-bottom:15px;
    color:#67ff9b;
    font-size:28px;
}

.card p{
    line-height:1.8;
    opacity:0.9;
}

/* STATS */
.stats{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:25px;
    margin-top:60px;
}

.stat-box{
    background:linear-gradient(145deg,#0c3020,#123b28);
    padding:40px 20px;
    border-radius:25px;
    text-align:center;
    transition:0.3s;
}

.stat-box:hover{
    transform:scale(1.05);
}

.stat-box h2{
    font-size:55px;
    color:#67ff9b;
}

.stat-box p{
    margin-top:15px;
    font-size:18px;
}

/* TIMELINE */
.timeline{
    border-left:4px solid #67ff9b;
    padding-left:30px;
    max-width:900px;
    margin:auto;
}

.timeline-item{
    margin-bottom:50px;
}

.timeline-item h3{
    color:#67ff9b;
    margin-bottom:10px;
}

/* PROBLEMER */
.problem-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:25px;
}

.problem-box{
    background:#111;
    border-radius:20px;
    padding:30px;
    border:1px solid rgba(255,255,255,0.08);
}

.problem-box ul{
    margin-top:20px;
    line-height:2;
}

/* FOOTER */
footer{
    text-align:center;
    padding:50px 20px;
    background:black;
}

footer h2{
    color:#67ff9b;
    margin-bottom:10px;
}

/* ANIMATION */
@keyframes fadeIn{
    from{
        opacity:0;
        transform:translateY(30px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

/* MOBILE */
@media(max-width:768px){

.hero-content h2{
    font-size:42px;
}

.section-title{
    font-size:36px;
}

nav ul{
    gap:15px;
    font-size:14px;
}

}
</style>
</head>
<body>

<nav>
    <h1>⚡ Future Energy</h1>

    <ul>
        <li><a href="#vind">Vind</a></li>
        <li><a href="#sol">Sol</a></li>
        <li><a href="#fakta">Fakta</a></li>
        <li><a href="#problemer">Problemer</a></li>
    </ul>
</nav>

<section class="hero">
    <div class="hero-content">
        <h2>Fremtidens Grønne Energi</h2>

        <p>
            Vindmøller og solceller hjælper verden med at skabe ren energi,
            reducere CO₂ og gøre fremtiden mere bæredygtig.
        </p>

        <a href="#vind" class="hero-btn">Udforsk Mere</a>
    </div>
</section>

<section id="vind">

<h1 class="section-title">Vindmøller</h1>

<div class="cards">

<div class="card">
<img src="https://images.unsplash.com/photo-1466611653911-95081537e5b7?q=80&w=1200&auto=format&fit=crop">

<div class="card-content">
<h3>Hvordan virker de?</h3>
<p>
Vindmøller omdanner vindens bevægelse til elektricitet.
Når vinden rammer vingerne, roterer generatoren og skaber strøm.
</p>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1497436072909-60f360e1d4b1?q=80&w=1200&auto=format&fit=crop">

<div class="card-content">
<h3>Bedste placeringer</h3>
<p>
Vindmøller fungerer bedst ved kyster, på åbne marker og offshore i havet,
hvor vinden er stærk og stabil.
</p>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1473341304170-971dccb5ac1e?q=80&w=1200&auto=format&fit=crop">

<div class="card-content">
<h3>Bæredygtighed</h3>
<p>
Vindenergi udleder næsten ingen CO₂ under drift og hjælper med at erstatte fossile brændstoffer.
</p>
</div>
</div>

</div>
</section>

<section id="sol">

<h1 class="section-title">Solceller</h1>

<div class="cards">

<div class="card">
<img src="https://images.unsplash.com/photo-1509391366360-2e959784a276?q=80&w=1200&auto=format&fit=crop">

<div class="card-content">
<h3>Hvordan virker de?</h3>
<p>
Solceller bruger solens lys til at producere elektricitet gennem fotovoltaiske celler.
</p>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1508514177221-188b1cf16e9d?q=80&w=1200&auto=format&fit=crop">

<div class="card-content">
<h3>Hvor skal de stå?</h3>
<p>
Solceller virker bedst på sydvendte tage og store områder med meget sollys.
</p>
</div>
</div>

<div class="card">
<img src="https://images.unsplash.com/photo-1497440001374-f26997328c1b?q=80&w=1200&auto=format&fit=crop">

<div class="card-content">
<h3>Fordele</h3>
<p>
Solenergi er stille, vedvarende og kan installeres næsten overalt.
</p>
</div>
</div>

</div>
</section>

<section id="fakta">

<h1 class="section-title">Live Fakta & Statistik</h1>

<div class="stats">

<div class="stat-box">
<h2 id="windCounter">0</h2>
<p>MWh produceret af vind i dag</p>
</div>

<div class="stat-box">
<h2 id="solarCounter">0</h2>
<p>MWh produceret af sol i dag</p>
</div>

<div class="stat-box">
<h2>67%</h2>
<p>Af dansk strøm kommer fra grøn energi</p>
</div>

<div class="stat-box">
<h2>0 CO₂</h2>
<p>Direkte udledning under produktion</p>
</div>

</div>
</section>

<section>
<h1 class="section-title">Udviklingen af Grøn Energi</h1>

<div class="timeline">

<div class="timeline-item">
<h3>1990</h3>
<p>Danmark begyndte at investere massivt i vindenergi.</p>
</div>

<div class="timeline-item">
<h3>2005</h3>
<p>Store offshore-vindmølleparker blev bygget i Nordsøen.</p>
</div>

<div class="timeline-item">
<h3>2020</h3>
<p>Solceller blev langt billigere og mere effektive.</p>
</div>

<div class="timeline-item">
<h3>2030</h3>
<p>Målet er at gøre energiforsyningen næsten helt grøn.</p>
</div>

</div>
</section>

<section id="problemer">

<h1 class="section-title">Problematikker</h1>

<div class="problem-grid">

<div class="problem-box">
<h2>Vindmøller</h2>

<ul>
<li>Kan larme i nogle områder</li>
<li>Påvirker fugle og natur</li>
<li>Nogle synes de ødelægger udsigten</li>
<li>Kræver meget plads offshore</li>
</ul>
</div>

<div class="problem-box">
<h2>Solceller</h2>

<ul>
<li>Virker dårligere om vinteren</li>
<li>Kræver sjældne materialer</li>
<li>Store solcelleparker tager plads</li>
<li>Kræver batterier til lagring</li>
</ul>
</div>

</div>
</section>

<footer>
<h2>⚡ Future Energy DK</h2>
<p>Lavet af Bunyamin • Grøn energi for fremtiden</p>
</footer>

<script>
let wind = 125000;
let solar = 48000;

setInterval(() => {
    wind += Math.floor(Math.random()*15);
    solar += Math.floor(Math.random()*8);

    document.getElementById('windCounter').innerText = wind.toLocaleString();
    document.getElementById('solarCounter').innerText = solar.toLocaleString();
}, 100);
</script>

</body>
</html>
```

## Sådan bruger du den

1. Opret en fil der hedder:

```txt
index.html
```

2. Kopiér ALT koden ind.

3. Åbn filen i browseren.

4. Upload den til GitHub Pages eller Netlify for at gøre den online.
