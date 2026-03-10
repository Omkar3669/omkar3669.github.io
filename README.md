<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BMW.com | The International BMW Website</title>
    <link rel="icon" href="https://www.bmw.com/etc.clientlibs/settings/wcm/designs/bmwcom/base/frontend/resources/img/favicon.ico">
    <style>
        :root {
            --bmw-blue: #0066b1;
            --bmw-m-light: #009ada;
            --bmw-m-dark: #003057;
            --bmw-m-red: #e7222e;
            --text-main: #262626;
            --text-secondary: #666;
            --bg-light: #f6f6f6;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: "BMWTypeNext", "Helvetica Neue", Helvetica, Arial, sans-serif;
            color: var(--text-main);
            background-color: #fff;
            line-height: 1.5;
        }

        /* --- NAVIGATION --- */
        nav {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px 5%;
            background: #fff;
            border-bottom: 1px solid #e5e5e5;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-left { display: flex; align-items: center; gap: 40px; }
        
        .logo-box img {
            width: 50px;
            height: 50px;
        }

        .nav-links { display: flex; gap: 25px; }
        .nav-links a {
            text-decoration: none;
            color: var(--text-main);
            font-size: 14px;
            font-weight: 400;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* --- HERO SECTION --- */
        .hero {
            position: relative;
            height: 90vh;
            background: url('https://next-media.bmw.com/p/m/v1/public/contents/editorial/bmw-m/2024/m5-sedan/teaser/bmw-m5-sedan-teaser-sp-xxl.jpg') center/cover no-repeat;
            display: flex;
            align-items: center;
            color: #fff;
        }

        .hero-overlay {
            padding-left: 8%;
            max-width: 700px;
        }

        .hero-overlay h2 { font-size: 1.2rem; font-weight: 300; letter-spacing: 4px; margin-bottom: 10px; }
        .hero-overlay h1 { font-size: 4.5rem; font-weight: 300; line-height: 1.1; margin-bottom: 30px; }

        .btn-primary {
            display: inline-block;
            padding: 15px 40px;
            background: var(--bmw-blue);
            color: #fff;
            text-decoration: none;
            font-weight: bold;
            font-size: 14px;
            transition: 0.3s;
        }
        .btn-primary:hover { background: #004a80; }

        /* --- M STRIPES --- */
        .m-stripes { height: 6px; display: flex; }
        .s1 { flex: 1; background: var(--bmw-m-light); }
        .s2 { flex: 1; background: var(--bmw-m-dark); }
        .s3 { flex: 1; background: var(--bmw-m-red); }

        /* --- CONTENT SECTIONS --- */
        .container { padding: 80px 8%; }
        
        .label {
            font-size: 12px;
            letter-spacing: 2px;
            color: var(--text-secondary);
            text-transform: uppercase;
            margin-bottom: 10px;
            display: block;
        }

        h2.section-title {
            font-size: 2.5rem;
            font-weight: 300;
            margin-bottom: 50px;
        }

        /* --- THE GRID --- */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
            gap: 2px; /* BMW uses tight spacing */
            background: #e5e5e5; /* Border color for the grid */
            border: 1px solid #e5e5e5;
        }

        .card {
            background: #fff;
            padding: 0;
            overflow: hidden;
            position: relative;
        }

        .card img {
            width: 100%;
            height: 450px;
            object-fit: cover;
            transition: transform 0.8s ease;
        }

        .card:hover img { transform: scale(1.05); }

        .card-info {
            position: absolute;
            bottom: 30px;
            left: 30px;
            color: white;
            text-shadow: 0 2px 10px rgba(0,0,0,0.5);
        }

        .card-info h3 { font-size: 1.8rem; font-weight: 300; }

        /* --- FOOTER --- */
        footer {
            background: #111;
            color: #fff;
            padding: 80px 8% 40px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            margin-bottom: 60px;
        }

        .footer-col h4 { margin-bottom: 20px; font-size: 14px; text-transform: uppercase; color: #888; }
        .footer-col ul { list-style: none; }
        .footer-col ul li { margin-bottom: 10px; font-size: 14px; cursor: pointer; }

        @media (max-width: 768px) {
            .hero-overlay h1 { font-size: 2.5rem; }
            .grid { grid-template-columns: 1fr; }
            .footer-grid { grid-template-columns: 1fr 1fr; gap: 30px; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="nav-left">
            <div class="logo-box">
                <img src="https://upload.wikimedia.org/wikipedia/commons/4/44/BMW.svg" alt="BMW Logo">
            </div>
            <div class="nav-links">
                <a href="#">Models</a>
                <a href="#">Electric</a>
                <a href="#">Circular World</a>
                <a href="#">Motorrad</a>
            </div>
        </div>
        <div class="nav-right">
            <span style="font-size: 20px; cursor: pointer;">🔍</span>
        </div>
    </nav>

    <section class="hero">
        <div class="hero-overlay">
            <h2>M HYBRID.</h2>
            <h1>THE ALL-NEW <br> BMW M5.</h1>
            <a href="#" class="btn-primary">DISCOVER NOW</a>
        </div>
    </section>

    <div class="m-stripes">
        <div class="s1"></div><div class="s2"></div><div class="s3"></div>
    </div>

    <div class="container">
        <span class="label">Sheer Driving Pleasure</span>
        <h2 class="section-title">Explore the lineup</h2>

        <div class="grid">
            <div class="card">
                <img src="https://images.unsplash.com/photo-1603386329225-868f9b1ee6c9?q=80&w=2069" alt="BMW M8">
                <div class="card-info">
                    <p>M-Series</p>
                    <h3>The M8 Competition</h3>
                </div>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1556122071-e404be74749f?q=80&w=2070" alt="BMW i7">
                <div class="card-info">
                    <p>Electric</p>
                    <h3>The All-Electric i7</h3>
                </div>
            </div>

            <div class="card">
                <img src="https://images.unsplash.com/photo-1615172282427-9a57ef2d142e?q=80&w=2070" alt="BMW S1000RR">
                <div class="card-info">
                    <p>Motorrad</p>
                    <h3>S 1000 RR</h3>
                
