<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cineemanch | Movie Reviews & Analysis</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-deep: #0a0a0b;
            --sidebar-bg: #121214;
            --accent-red: #e50914;
            --text-dim: #b3b3b3;
        }

        body {
            background-color: var(--bg-deep);
            color: white;
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }

        /* 1. Header & Banner */
        .banner-wrapper {
            width: 100%;
            background-color: var(--bg-deep);
            border-bottom: 2px solid var(--accent-red);
            overflow: hidden;
        }

        .hero-banner {
            width: 100%;
            max-height: 400px;
            object-fit: cover;
            display: block;
            mask-image: linear-gradient(to bottom, black 80%, transparent 100%);
            -webkit-mask-image: linear-gradient(to bottom, black 80%, transparent 100%);
        }

        /* 2. Column Layout Setup */
        .app-container {
            display: flex;
            flex-direction: row;
            min-height: 100vh;
        }

        /* Sidebar */
        .side-nav {
            flex: 0 0 260px;
            background-color: var(--sidebar-bg);
            position: sticky;
            top: 0;
            height: 100vh;
            border-right: 1px solid #2d2d2d;
            padding: 2rem;
        }

        .brand-title {
            font-weight: 800;
            color: var(--accent-red);
            font-size: 1.4rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 2.5rem;
            display: block;
            text-decoration: none;
        }

        .nav-link {
            color: var(--text-dim);
            font-weight: 600;
            padding: 0.8rem 1rem;
            border-radius: 8px;
            transition: 0.3s;
            margin-bottom: 0.5rem;
            display: block;
            text-decoration: none;
        }

        .nav-link:hover, .nav-link.active {
            background: rgba(229, 9, 20, 0.1);
            color: var(--accent-red);
        }

        /* Main Center Content */
        .main-content { 
            flex: 1;
            padding: 2.5rem; 
        }

        .video-spotlight {
            background: #1a1d20;
            border-radius: 16px;
            padding: 1.5rem;
            border: 1px solid #333;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            margin-top: 20px;
        }

        /* Right Feed */
        .right-feed {
            flex: 0 0 300px;
            height: 100vh;
            position: sticky;
            top: 0;
            padding: 2rem;
            border-left: 1px solid #2d2d2d;
            overflow-y: auto;
        }

        .feed-item {
            background: #1a1d20;
            border-radius: 10px;
            padding: 1rem;
            margin-bottom: 1.2rem;
            border-left: 4px solid var(--accent-red);
            transition: 0.2s;
        }

        .feed-item:hover { transform: translateX(5px); }

        @media (max-width: 992px) {
            .app-container { flex-direction: column; }
            .side-nav, .right-feed { height: auto; position: relative; border: none; padding: 1.5rem; flex: none; }
            .hero-banner { max-height: 200px; }
        }
    </style>
</head>
<body>

    <header class="banner-wrapper">
        <img src="Modern Gaming Cover YouTube Channel Art-2.png" alt="Cineemanch Banner" class="hero-banner">
    </header>

    <div class="app-container">
        <nav class="side-nav">
            <div class="brand-title">CINEEMANCH</div>
            <a href="#" class="nav-link active">HOME</a>
            <a href="#" class="nav-link">MOVIE REVIEWS</a>
            <a href="#" class="nav-link">WRITTEN BLOG</a>
            <a href="https://www.youtube.com/@cineemanch" class="nav-link" target="_blank">YOUTUBE CHANNEL</a>
        </nav>

        <main class="main-content">
            <h2 class="text-uppercase">Featured Review</h2>
            <section class="video-spotlight">
                <div class="ratio ratio-16x9 mb-3" style="background:#000; height: 300px; border-radius: 8px; display:flex; align-items:center; justify-content:center;">
                   <p class="text-muted">Video Placeholder</p>
                </div>
                <h3>The Batman: A Visual Masterclass</h3>
                <p class="text-dim">Does Matt Reeves' vision hold up under the Cineemanch lens? We break down the lighting, the score, and the soul of Gotham.</p>
            </section>
        </main>

        <aside class="right-feed">
            <h4 class="mb-3">Latest Blog Posts</h4>
            <div class="feed-item">
                <span class="badge bg-danger mb-2">9.5/10</span>
                <h6>The Technical Brilliance of Batman</h6>
                <p class="small text-muted">A written deep-dive into cinematography...</p>
            </div>
            </aside>
    </div>

</body>
</html>
