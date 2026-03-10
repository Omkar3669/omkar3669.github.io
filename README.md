<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BMW | Luxury Cars & Motorcycles</title>
    <style>
        /* BMW Official Color Palette */
        :root {
            --white: #ffffff;
            --light-grey: #f2f2f2;
            --medium-grey: #666666;
            --dark-grey: #262626;
            --bmw-blue: #0066b1;
            --bmw-m-light: #009ada;
            --bmw-m-dark: #003057;
            --bmw-m-red: #e7222e;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }

        body {
            font-family: "BMWTypeNext", "Helvetica Neue", Helvetica, Arial, sans-serif;
            background-color: var(--white);
            color: var(--dark-grey);
            -webkit-font-smoothing: antialiased;
        }

        /* Top Bar & Nav */
        nav {
            height: 80px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0 5%;
            background: white;
            border-bottom: 1px solid #e5e5e5;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo-container { display: flex; align-items: center; }
        .logo-img { height: 50px; width: 50px; margin-right: 15px; }

        .nav-links a {
            text-decoration: none;
            color: var(--dark-grey);
            font-weight: 500;
            font-size: 14px;
            margin-left: 30px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* Hero Banner */
        .hero {
            position: relative;
            height: 85vh;
            background: url('https://images.unsplash.com/photo-1555215695-3004980ad54e?q=80&w=2070') center/cover no-repeat;
            display: flex;
            align-items: flex-end;
            padding: 80px 5%;
        }

        .hero-content {
            color: white;
            max-width: 600px;
        }

        .hero-content h1 { font-size: 3rem; font-weight: 300; margin-bottom: 20px; }

        .btn-white {
            background: white;
            color: black;
            padding: 12px 35px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
            transition: 0.3s;
        }

        /* M-Performance Stripes Divider */
        .m-stripes {
            height: 5px;
            display: flex;
            width: 100%;
        }
        .s1 { width: 33.3%; background: var(--bmw-m-light); }
        .s2 { width: 33.3%; background: var(--bmw-m-dark); }
        .s3 { width: 33.3%; background: var(--bmw-m-red); }

        /* Model Grid */
        .section-container { padding: 80px 5%; }
        .section-header { margin-bottom: 40px; }
        .section-header h2 { font-size: 2rem; font-weight: 300; }

        .model-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 20px;
        }

        .model-card {
            background: var(--light-grey);
            padding: 40px;
            transition: 0.4s;
            cursor: pointer;
            position: relative;
        }

        .model-card:hover { background: #e9e9e9; }
        .model-card img { width: 100%; height: auto; transition: 0.4s; }
        .model-card:hover img { transform: scale(1.05); }

        .model-info h3 { font-size: 1.5rem; margin-top: 20px; }
        .model-info p { color: var(--medium-grey); margin-bottom: 20px; }

        /* Footer */
        footer {
            background: var(--dark-grey);
            color: #ccc;
            padding: 60px 5%;
            text-align: center;
            font-size: 13px;
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo-container">
            <img class="logo-img" src="https://upload.wikimedia.org/wikipedia/commons/4/44/BMW.svg" alt="BMW Logo">
            <span style="font-weight:bold; letter-spacing: 2px;">Sheer Driving Pleasure</span>
        </div>
        <div class="nav-links">
            <a href="#models">Models</a>
            <a href="#motorrad">Motorrad</a>
            <a href="#">Electric</a>
        </div>
    </nav>

    <div class="hero">
        <div class="hero-content">
            <h1>THE ALL-NEW BMW M5</h1>
            <p style="margin-bottom: 25px;">Engineered for adrenaline. Crafted for luxury.</p>
            <a href="#" class="btn-white">DISCOVER MORE</a>
        </div>
    </div>

    <div class="m-stripes">
        <div class="s1"></div><div class="s2"></div><div class="s3"></div>
    </div>

    <div class="section-container" id="models">
        <div class="section-header">
            <p>CHOOSE YOUR ENGINE</p>
            <h2>BMW MODELS</h2>
        </div>

        <div class="model-grid">
            <div class="model-card">
                <div class="model-info">
                    <p>M Performance</p>
                    <h3>The M4 Coupe</h3>
                </div>
                <img src="https://images.unsplash.com/photo-1619362224246-70150d1804d8?q=80&w=1000" alt="BMW M4">
            </div>

            <div class="model-card">
                <div class="model-info">
                    <p>Luxury Sedan</p>
                    <h3>The 7 Series</h3>
                </div>
                <img src="https://images.unsplash.com/photo-1549399542-7e3f8b79c341?q=80&w=1000" alt="BMW 7">
            </div>
        </div>
    </div>

    <div class="section-container" id="motorrad" style="background: #fafafa;">
        <div class="section-header">
            <p>TWO WHEELS. ONE PASSION.</p>
            <h2>BMW MOTORRAD</h2>
        </div>

        <div class="model-grid">
            <div class="model-card" style="background: white;">
                <div class="model-info">
                    <p>Sport</p>
                    <h3>S 1000 RR</h3>
                </div>
                <img src="https://images.unsplash.com/photo-1568772585407-9361f9bf3a87?q=80&w=1000" alt="S1000RR">
            </div>

            <div class="model-card" style="background: white;">
                <div class="model-info">
                    <p>Adventure</p>
                    <h3>R 1300 GS</h3>
                </div>
                <img src="https://images.unsplash.com/photo-1591637333184-19aa84b3e01f?q=80&w=1000" alt="R1250GS">
            </div>
        </div>
    </div>

    <footer>
        <p>© BMW AG 2026. Note: This is a fan-made website for portfolio purposes.</p>
    </footer>

</body>
</html>
