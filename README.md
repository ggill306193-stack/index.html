# index.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Explore Yellowstone National Park - Made by Gurpinder Gill</title>
  <style>
    /* Base styles */
    body {
      font-family: "Segoe UI", Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f4f4f4;
      scroll-behavior: smooth;
      color: #333;
    }

    /* Side borders with pattern */
    body::before, body::after {
      content: "";
      position: fixed;
      top: 0;
      bottom: 0;
      width: 15px;
      background: #2e8b57 url('https://www.transparenttextures.com/patterns/lines.png') repeat-y;
      z-index: 999;
    }
    body::before { left: 0; }
    body::after { right: 0; }

    /* Top banner */
    .submission {
      background: #ffeb3b;
      color: black;
      padding: 15px;
      text-align: center;
      font-weight: bold;
      font-size: 18px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }

    /* Header with overlay */
    header {
      background: url('https://upload.wikimedia.org/wikipedia/commons/6/60/Old_Faithful_erupting.jpg') no-repeat center center/cover;
      color: white;
      height: 65vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      position: relative;
    }
    header::after {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(0,0,0,0.45);
    }
    header h1, header p, header a {
      position: relative;
      z-index: 1;
    }
    header h1 {
      font-size: 3rem;
      margin-bottom: 0.5em;
      background: linear-gradient(90deg, #ffdd00, #ff6600);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: fadeInDown 1s ease forwards;
    }
    header p {
      color: #ffdddd;
      font-size: 1.2rem;
      margin-bottom: 1em;
      animation: fadeInUp 1.5s ease forwards;
    }

    /* Nav bar */
    nav {
      background: #333;
      padding: 1em;
      position: sticky;
      top: 0;
      z-index: 1000;
      display: flex;
      justify-content: center;
      gap: 1.5em;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #ff6600;
    }

    /* Sections */
    section {
      padding: 3em 1.5em;
      max-width: 1100px;
      margin: auto;
      line-height: 1.6;
    }
    section h2 {
      text-align: center;
      margin-bottom: 1.2em;
      font-size: 2rem;
      position: relative;
    }
    section h2::after {
      content: "";
      display: block;
      width: 80px;
      height: 4px;
      margin: 0.5em auto;
      background: #2e8b57;
      border-radius: 2px;
    }
    .attraction, .avoid {
      margin-bottom: 1.5em;
      padding: 1em;
      border-left: 4px solid #2e8b57;
      background: white;
      border-radius: 8px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .attraction:hover, .avoid:hover {
      transform: translateY(-4px);
      box-shadow: 0 6px 16px rgba(0,0,0,0.15);
    }

    /* Buttons */
    .button {
      padding: 0.6em 1.2em;
      background: #ff6600;
      color: white;
      text-decoration: none;
      border-radius: 25px;
      font-weight: bold;
      margin: 0.3em;
      transition: background 0.3s, transform 0.2s;
    }
    .button:hover {
      background: #e65c00;
      transform: scale(1.05);
    }

    /* Gallery */
    .gallery {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      justify-content: center;
    }
    .gallery img {
      width: 100%;
      max-width: 320px;
      border-radius: 12px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .gallery img:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    }

    /* Footer */
    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 1em;
      font-size: 0.9rem;
    }

    /* Animations */
    @keyframes fadeInDown {
      from {opacity: 0; transform: translateY(-30px);}
      to {opacity: 1; transform: translateY(0);}
    }
    @keyframes fadeInUp {
      from {opacity: 0; transform: translateY(30px);}
      to {opacity: 1; transform: translateY(0);}
    }
  </style>
</head>
<body>
  <div class="submission">
    Submitted To Mr. Steven Wine By Gurpinder Gill
  </div>

  <header>
    <h1>Explore Yellowstone National Park</h1>
    <p>America’s first National Park – geysers, wildlife, and breathtaking scenery</p>
    <a class="button" href="#things-to-do">Things To Do</a>
    <a class="button" href="#things-to-avoid">Things To Avoid</a>
  </header>

  <nav>
    <a href="#history">History & Biography</a>
    <a href="#things-to-do">Things To Do</a>
    <a href="#things-to-avoid">Things To Avoid</a>
    <a href="#gallery">Gallery</a>
  </nav>

  <section id="history">
    <h2>The Story of Yellowstone</h2>
    <p>Yellowstone National Park, established in 1872, spans Wyoming, Montana, and Idaho. It was the first National Park in the world, created to protect its geothermal wonders and wildlife.</p>
    <p>Native American tribes lived in the Yellowstone region for thousands of years, hunting, fishing, and gathering plants. The park sits atop a supervolcano, featuring geysers, hot springs, and mud pots.</p>
    <ul>
      <li>Over 10,000 geothermal features</li>
      <li>Home to bison, grizzly bears, wolves, and elk</li>
      <li>Grand Prismatic Spring is the largest hot spring in the U.S.</li>
    </ul>
  </section>

  <section id="things-to-do">
    <h2>Top Attractions & Activities</h2>
    <div class="attraction">
      <h3>Old Faithful Geyser</h3>
      <p>Watch eruptions every 90 minutes. A must-see natural spectacle.</p>
    </div>
    <div class="attraction">
      <h3>Grand Prismatic Spring</h3>
      <p>Rainbow-colored hot spring; perfect for photos.</p>
    </div>
    <div class="attraction">
      <h3>Yellowstone Lake</h3>
      <p>Boating, fishing, and lakeside views.</p>
    </div>
    <div class="attraction">
      <h3>Wildlife Watching in Lamar Valley</h3>
      <p>See bison, elk, and wolves; best in early morning.</p>
    </div>
    <div class="attraction">
      <h3>Hiking Trails</h3>
      <p>Fairy Falls, Mount Washburn, and more; scenic trails for all skill levels.</p>
    </div>
    <div class="attraction">
      <h3>Grand Canyon of Yellowstone & Lower Falls</h3>
      <p>Iconic waterfall vistas.</p>
    </div>
  </section>

  <section id="things-to-avoid">
    <h2>Stay Safe and Respect Yellowstone</h2>
    <div class="avoid">
      <h3>Feeding Wildlife</h3>
      <p>Dangerous for humans and animals; heavy fines apply.</p>
    </div>
    <div class="avoid">
      <h3>Going Off-Trail</h3>
      <p>Thermal features can burn through the crust.</p>
    </div>
    <div class="avoid">
      <h3>Visiting in Harsh Winter</h3>
      <p>Snow blocks roads; hypothermia risk.</p>
    </div>
    <div class="avoid">
      <h3>Ignoring Park Rules</h3>
      <p>Littering, fireworks, and camping in non-designated areas harms the park.</p>
    </div>
    <div class="avoid">
      <h3>Crowds at Old Faithful</h3>
      <p>Visit early or late to avoid congestion.</p>
    </div>
  </section>

  <section id="gallery">
    <h2>Gallery</h2>
    <div class="gallery">
      <img src="https://jacksonhole-traveler-production.s3.amazonaws.com/wp-content/uploads/2014/05/old-faithful-4OFS1059-1280x853.jpg" alt="Experiencing the Old Faithful Geyser Basin - Jackson Hole Traveler"/>
      <img src="https://d.newsweek.com/en/full/2379240/yellowstone-lake.jpg" alt="Yellowstone Lake Ice Cover Unchanged—but 'Tipping Point' Is ..."/>
      <img src="https://www.tetonscience.org/wp-content/uploads/2020/09/SE-Sunset-in-Lamar-scaled-1.jpg" alt="Battle of the Yellowstone Wildlife Valleys: Hayden Valley vs ..."/>
      <img src="https://muir-way.com/cdn/shop/articles/yellowstone-image.jpg?v=1746480606&amp;width=5464" alt="Exploring Yellowstone's Geology: Features, History, &amp; More – Muir Way"/>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Explore Yellowstone. Made by Gurpinder Gill. All rights reserved.</p>
  </footer>
</body>
</html>
