# saikiavicky43-ui.github.io
Official poetry website of Vicky Saikia
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080808">

<title>Vicky Saikia | Poetry & Feelings</title>

<meta name="description" content="Official poetry website of Vicky Saikia. Assamese and Hindi poetry, memories and emotions.">

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600;700&family=Poppins:wght@300;400;500;600&family=Noto+Serif+Bengali:wght@400;500;600&display=swap" rel="stylesheet">

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  background: #080808;
  color: #eeeeee;
  font-family: 'Poppins', sans-serif;
  overflow-x: hidden;
}

a {
  color: inherit;
  text-decoration: none;
}

/* Main layout */

.layout {
  display: grid;
  grid-template-columns: 230px minmax(0, 1fr) 310px;
  min-height: 100vh;
  gap: 25px;
  padding: 25px;
}

/* Left sidebar */

.sidebar {
  position: sticky;
  top: 25px;
  height: calc(100vh - 50px);
  background: #111111;
  border: 1px solid #202020;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 25px 15px;
}

.small-title {
  font-size: 10px;
  letter-spacing: 5px;
  color: #aaaaaa;
  margin-bottom: 18px;
}

.sidebar h1 {
  font-family: 'Playfair Display', serif;
  font-size: 38px;
  font-weight: 500;
  line-height: 1.3;
}

.tagline {
  font-size: 12px;
  color: #aaaaaa;
  margin-top: 12px;
  line-height: 1.8;
}

nav {
  display: flex;
  flex-direction: column;
  gap: 22px;
  margin-top: 45px;
}

nav a {
  font-size: 12px;
  letter-spacing: 1px;
  color: #bbbbbb;
  transition: .3s;
}

nav a:hover {
  color: white;
}

/* Main content */

main {
  min-width: 0;
  max-width: 850px;
  width: 100%;
  margin: auto;
}

.hero {
  padding: 55px 10px 35px;
}

.hero h2 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(32px, 5vw, 48px);
  font-weight: 400;
  line-height: 1.3;
  margin-bottom: 18px;
}

.hero p {
  color: #999999;
  font-size: 14px;
  line-height: 2;
  max-width: 500px;
}

.section-title {
  font-family: 'Playfair Display', serif;
  font-size: 25px;
  font-weight: 400;
  margin: 15px 0 25px;
}

/* Search */

.search {
  width: 100%;
  padding: 15px;
  background: #151515;
  color: white;
  border: 1px solid #292929;
  outline: none;
  border-radius: 7px;
  margin-bottom: 25px;
  font-family: inherit;
}

.search:focus {
  border-color: #777777;
}

/* Poetry cards */

.poems {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 18px;
}

.poem {
  background: #141414;
  border: 1px solid #222222;
  border-radius: 9px;
  padding: 25px 22px;
  transition: .3s;
  min-width: 0;
}

.poem:hover {
  background: #1b1b1b;
  transform: translateY(-3px);
}

.category {
  font-size: 9px;
  letter-spacing: 1px;
  color: #777777;
  margin-bottom: 15px;
  text-transform: uppercase;
}

.poem h3 {
  font-family: 'Noto Serif Bengali', 'Playfair Display', serif;
  font-size: 21px;
  font-weight: 500;
  margin-bottom: 15px;
}

.poem p {
  font-family: 'Noto Serif Bengali', serif;
  font-size: 14px;
  color: #bdbdbd;
  line-height: 2;
  white-space: pre-line;
}

/* Featured poetry */

.featured {
  background: #141414;
  border: 1px solid #252525;
  border-radius: 10px;
  padding: 28px 25px;
  margin-top: 20px;
}

.featured h2 {
  font-family: 'Playfair Display', serif;
  font-size: 25px;
  margin: 15px 0;
}

.featured p {
  font-family: 'Noto Serif Bengali', serif;
  font-size: 15px;
  color: #c4c4c4;
  line-height: 2.2;
  white-space: pre-line;
}

/* About */

.about {
  text-align: center;
  padding: 65px 15px;
}

.about h2 {
  font-family: 'Playfair Display', serif;
  font-size: 28px;
  font-weight: 400;
  margin-bottom: 20px;
}

.about p {
  font-size: 14px;
  color: #999999;
  line-height: 2.2;
}

/* Right featured column */

.right-panel {
  position: sticky;
  top: 25px;
  align-self: start;
  background: #121212;
  border: 1px solid #242424;
  border-radius: 9px;
  padding: 25px 22px;
}

.right-panel h3 {
  font-family: 'Playfair Display', serif;
  font-size: 22px;
  margin: 15px 0;
}

.right-panel p {
  font-family: 'Noto Serif Bengali', serif;
  font-size: 14px;
  color: #bbbbbb;
  line-height: 2.1;
  white-space: pre-line;
}

.date {
  color: #777777;
  font-size: 11px;
  margin-top: 20px;
}

footer {
  border-top: 1px solid #222222;
  padding: 25px 10px;
  text-align: center;
  color: #777777;
  font-size: 11px;
}

/* Mobile responsive */

@media (max-width: 900px) {

  .layout {
    grid-template-columns: 190px minmax(0, 1fr);
  }

  .right-panel {
    grid-column: 2;
    position: static;
  }

}

@media (max-width: 600px) {

  .layout {
    display: flex;
    flex-direction: column;
    padding: 15px;
    gap: 18px;
  }

  .sidebar {
    position: static;
    width: 100%;
    height: auto;
    padding: 25px 15px;
  }

  .sidebar h1 {
    font-size: 32px;
  }

  nav {
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;
    gap: 25px;
    margin-top: 22px;
  }

  main {
    width: 100%;
  }

  .hero {
    padding: 35px 5px 25px;
  }

  .hero h2 {
    font-size: 34px;
  }

  .section-title {
    font-size: 23px;
  }

  .poems {
    grid-template-columns: 1fr;
    gap: 15px;
  }

  .poem {
    padding: 23px 20px;
  }

  .poem h3 {
    font-size: 22px;
  }

  .poem p {
    font-size: 14px;
    line-height: 2;
  }

  .featured {
    padding: 24px 20px;
  }

  .right-panel {
    width: 100%;
    position: static;
    padding: 22px;
  }

  .about {
    padding: 45px 10px;
  }

  footer {
    margin-top: 10px;
  }

}
</style>
</head>

<body>

<div class="layout">

<!-- LEFT SIDEBAR -->

<aside class="sidebar" id="home">

  <div class="small-title">A WORLD OF WORDS & FEELINGS</div>

  <h1>Vicky<br>Saikia</h1>

  <p class="tagline">
    Poetry • Memories • Emotions
  </p>

  <nav>
    <a href="#home">HOME</a>
    <a href="#poems">POEMS</a>
    <a href="#about">ABOUT</a>
  </nav>

</aside>

<!-- MAIN CONTENT -->

<main>

  <section class="hero">
    <h2>Words That Feel<br>Like Memories.</h2>

    <p>
      Welcome to my little world.<br>
      Here, every word carries a feeling
      and every poem holds a memory.
    </p>
  </section>

  <section id="poems">

    <h2 class="section-title">My Poetry Collection</h2>

    <input
      type="text"
      class="search"
      id="search"
      placeholder="Search my poems..."
      aria-label="Search poems"
    >

    <div class="poems" id="poemList">

      <article class="poem">
        <div class="category">Assamese Poetry</div>
        <h3>নীৰৱ সন্ধিয়া</h3>
        <p>
নিশাৰ বুকুত সন্ধিয়া নামি অহা ক্ষণ,
নিঃশব্দতাই কয় বহু নোকোৱা কথা।
শব্দবোৰে বুজাই যায় সময়ৰ বুকুত,
অন্তৰবোৰে বিচাৰে মাথোঁ অলপ সান্ত্বনা।
        </p>
      </article>

      <article class="poem">
        <div class="category">Assamese Poetry</div>
        <h3>স্মৃতি</h3>
        <p>
সময় পাৰ হৈ যায়, স্মৃতি নাযায়,
কিছুমান মানুহ মনৰ পৰা হেৰাই নাযায়।
নীৰৱতাৰ মাজতো কিছুমান কথা থাকে,
যিবোৰে কেৱল হৃদয়কেই চুই যায়।
        </p>
      </article>

      <article class="poem">
        <div class="category">Hindi Poetry</div>
        <h3>ख़ामोशी</h3>
        <p>
कुछ बातें लफ़्ज़ों में बयां नहीं होती,
कुछ यादें कभी पुरानी नहीं होती।
वक्त बदल जाता है अपनी रफ्तार से,
मगर कुछ एहसास कभी खत्म नहीं होते।
        </p>
      </article>

    </div>

    <p id="noResults" style="display:none;color:#999;padding:20px;">
      No poems found.
    </p>

  </section>

  <!-- ABOUT -->

  <section class="about" id="about">

    <h2>About The Author</h2>

    <p>
      I am Vicky Saikia.<br>
      A lover of words, poetry and emotions.<br>
      This is my little corner of the internet,
      where feelings find their way into words.
    </p>

  </section>

  <footer>
    © 2026 Vicky Saikia · All Rights Reserved
  </footer>

</main>

<!-- RIGHT FEATURED POEM -->

<aside class="right-panel">

  <div class="category">NEW • ASSAMESE POETRY</div>

  <h3>Ubhoti Ohar Opekkhat...</h3>

  <p>
আজিও কলমটো হাতত লৈ বহিছোঁ,
অথচ শব্দবোৰ আজি বৰ অচিনাকি।

কি লিখোঁ বাৰু এনে এটা কবিতা,
যাৰ প্ৰতিটো শাৰিত থাকে হৃদয় কপি উঠে।

আৰু তাই এবাৰ উভতি আহিব বুলি
ভাবি থকা মনটোৱে আজিও অপেক্ষা কৰে।

মই কোনো নতুন কাহিনী বিচৰা নাই,
পুৰণি অধ্যায়তে আকৌ এবাৰ মিলিব বিচাৰোঁ।

জোন তৰাই হাঁহিলে মোৰ পৃথিৱীখনো হাঁহিছিল।

এতিয়া মাথোঁ এটাই প্ৰাৰ্থনা—
যদি কেতিয়াবা মোৰ এই কবিতাই তাইৰ চকুত পৰে,
তেন্তে শব্দবোৰৰ মাজত লুকাই থকা মনুহজনক চিনি পাব...
  </p>

  <div class="date">
    — Vicky Saikia | 30 Oct 2026
  </div>

</aside>

</div>

<script>
const search = document.getElementById("search");
const poems = document.querySelectorAll(".poem");
const noResults = document.getElementById("noResults");

search.addEventListener("input", function() {

  const value = this.value.toLowerCase();
  let count = 0;

  poems.forEach(function(poem) {

    const match = poem.innerText.toLowerCase().includes(value);

    poem.style.display = match ? "" : "none";

    if (match) count++;

  });

  noResults.style.display = count === 0 ? "block" : "none";

});
</script>

</body>
</html>
