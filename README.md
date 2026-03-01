<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parvez Hossain Alif · awesome MERN+ profile</title>
    <!-- Font Awesome 6 (free) for extra polish -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- GitHub Markdown style (optional, for nice fallback) but we'll use our own modern look -->
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
        }
        body {
            background: #0a0c10;
            display: flex;
            justify-content: center;
            padding: 2rem 1rem;
            color: #c9d1d9;
        }
        .profile-card {
            max-width: 1100px;
            width: 100%;
            background: #0d1117;
            border-radius: 32px;
            border: 1px solid #30363d;
            box-shadow: 0 20px 40px rgba(0,0,0,0.8);
            overflow: hidden;
            backdrop-filter: blur(2px);
        }
        .banner img {
            width: 100%;
            max-height: 280px;
            object-fit: cover;
            border-bottom: 2px solid #2dba7e30;
            display: block;
        }
        .content {
            padding: 2rem 2.5rem 3rem;
        }
        h1 {
            font-size: 3rem;
            font-weight: 700;
            letter-spacing: -0.5px;
            background: linear-gradient(135deg, #b3e5fc, #a3e0ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 0.25rem;
        }
        .subhead {
            font-size: 1.35rem;
            color: #8b949e;
            font-weight: 400;
            border-left: 4px solid #2dba7e;
            padding-left: 1.5rem;
            margin: 0.5rem 0 1.5rem 0;
        }
        .badge-row {
            display: flex;
            flex-wrap: wrap;
            gap: 0.75rem;
            margin: 1.5rem 0 2rem 0;
        }
        .badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: #1f2937;
            padding: 0.6rem 1.4rem;
            border-radius: 40px;
            border: 1px solid #3c444d;
            font-weight: 500;
            color: #e6edf3;
            text-decoration: none;
            transition: 0.2s;
            font-size: 0.95rem;
        }
        .badge i {
            color: #2dba7e;
            font-size: 1.1rem;
        }
        .badge:hover {
            border-color: #2dba7e;
            background: #1e2a36;
            transform: translateY(-2px);
        }
        .section-title {
            font-size: 1.8rem;
            font-weight: 600;
            margin: 2.5rem 0 1.2rem 0;
            display: flex;
            align-items: center;
            gap: 12px;
            border-bottom: 2px solid #21262d;
            padding-bottom: 0.6rem;
        }
        .section-title i {
            color: #2dba7e;
            font-size: 2rem;
        }
        .grid-2col {
            display: grid;
            grid-template-columns: repeat(2,1fr);
            gap: 1.8rem;
        }
        .skill-block {
            background: #161b22;
            border-radius: 24px;
            padding: 1.8rem;
            border: 1px solid #30363d;
            box-shadow: 0 8px 0 #0a0c10;
        }
        .skill-block h3 {
            font-size: 1.5rem;
            margin-bottom: 1.2rem;
            color: #f0f6fc;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .skill-icons {
            display: flex;
            flex-wrap: wrap;
            gap: 14px;
            align-items: center;
        }
        .skill-icons img, .custom-icon {
            height: 40px;
            width: auto;
            transition: 0.2s;
            filter: drop-shadow(0 2px 4px #00000060);
        }
        .custom-icon {
            background: #1f2a36;
            padding: 0.5rem 1rem;
            border-radius: 30px;
            color: white;
            font-weight: 600;
            font-size: 0.9rem;
            display: inline-flex;
            align-items: center;
            gap: 6px;
            border: 1px solid #3b4450;
        }
        .custom-icon i {
            font-size: 1.2rem;
            color: #2dba7e;
        }
        .mermaid-box {
            background: #161b22;
            border-radius: 24px;
            padding: 1.8rem;
            border: 1px solid #2dba7e30;
            margin: 2rem 0;
            font-family: 'Fira Code', monospace;
        }
        .mermaid {
            color: #e6edf3;
            background: #0d1117;
            padding: 1.5rem;
            border-radius: 16px;
            border: 1px dashed #2dba7e;
            font-size: 0.9rem;
            line-height: 1.8;
            white-space: pre-wrap;
            word-break: break-word;
        }
        .stats-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin: 2.5rem 0 1rem;
        }
        .stat-item {
            background: #161b22;
            padding: 1rem 2rem;
            border-radius: 60px;
            border: 1px solid #2dba7e40;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 12px;
            font-size: 1.2rem;
        }
        .stat-item i {
            color: #2dba7e;
        }
        .profile-footer {
            text-align: center;
            margin-top: 3rem;
            opacity: 0.8;
        }
        hr {
            border: 1px solid #292e34;
            margin: 2rem 0 1rem;
        }
        @media (max-width: 650px) {
            .content { padding: 1.5rem; }
            h1 { font-size: 2.2rem; }
            .grid-2col { grid-template-columns: 1fr; }
        }
        /* additional accent */
        .text-neon { color: #2dba7e; }
        i.fa-solid, i.fa-regular { color: inherit; }
    </style>
</head>
<body>
    <div class="profile-card">
        <!-- Banner image (as in original) -->
        <div class="banner">
            <img src="https://i.ibb.co.com/zTnGYKS7/github-banner.jpg" alt="Parvez's GitHub banner" onerror="this.style.backgroundColor='#1f3b4e'; this.src='data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTIwMCIgaGVpZ2h0PSIzMDAiIHZpZXdCb3g9IjAgMCAxMjAwIDMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjMjIyNzJlIi8+PHRleHQgeD0iNTAlIiB5PSI1MCUiIGZvbnQtc2l6ZT0iNDAiIGZpbGw9IiMyZGJhN2UiIHRleHQtYW5jaG9yPSJtaWRkbGUiIGR5PSIuM2VtIiBmb250LWZhbWlseT0ibW9ub3NwYWNlIj5QQVJWRVogSE9TU0FJTiBBTElGPC90ZXh0Pjwvc3ZnPg=='">
        </div>

        <div class="content">
            <!-- header with name + badges -->
            <h1>👋 Parvez Hossain Alif</h1>
            <div class="subhead">
                <i class="fa-solid fa-crown" style="color:#2dba7e;"></i> 
                Frontend · MERN · Next.js · TypeScript · Better‑Auth
            </div>

            <!-- badges (projects, linkedin, email) -->
            <div class="badge-row">
                <a href="https://github.com/Parvez141300?tab=repositories" class="badge"><i class="fa-brands fa-github"></i> Projects 10+</a>
                <a href="https://www.linkedin.com/in/parvez-hossain-alif/" class="badge"><i class="fa-brands fa-linkedin"></i> Connect</a>
                <a href="mailto:your-email@example.com" class="badge"><i class="fa-solid fa-envelope"></i> Email</a>
                <span class="badge"><i class="fa-solid fa-location-dot"></i> MERN • Next • Prisma</span>
            </div>

            <!-- About me (refreshed) -->
            <div class="section-title"><i class="fa-solid fa-user-astronaut"></i> 🚀 about me</div>
            <p style="font-size: 1.15rem; line-height: 1.7; background: #161b22; padding: 1.5rem; border-radius: 24px; border:1px solid #2dba7e20;">
                <i class="fa-solid fa-quote-left" style="color:#2dba7e; opacity:0.8;"></i> 
                I'm a <strong>Frontend & MERN stack developer</strong> with a growing arsenal including <strong>Next.js, TypeScript, Prisma, PostgreSQL, Shadcn/ui, and Better‑Auth</strong>. 
                I love crafting secure, full‑stack apps with elegant UI and robust authentication. 
                Currently pushing into edge deployment and serverless.
            </p>

            <!-- ✦ NEW SKILL SECTIONS – showing all required technologies ✦ -->
            <div class="section-title"><i class="fa-solid fa-code"></i> ⚡ core tech stack</div>
            <div class="grid-2col">
                <!-- column 1: frontend & UI -->
                <div class="skill-block">
                    <h3><i class="fa-solid fa-paint-brush" style="color:#2dba7e;"></i> Frontend</h3>
                    <div class="skill-icons">
                        <img src="https://skillicons.dev/icons?i=html,css,js,react,next,tailwind,ts" alt="icons">
                        <span class="custom-icon"><i class="fa-brands fa-bootstrap"></i> Bootstrap</span>
                        <span class="custom-icon"><i class="fa-solid fa-wand-magic-sparkles"></i> Shadcn/ui</span>
                        <span class="custom-icon"><i class="fa-solid fa-paint-roller"></i> DaisyUI</span>
                    </div>
                    <p style="margin-top: 1.2rem; color:#b1bac4;"><i class="fa-regular fa-circle-check text-neon"></i> Next.js 14, RSC, App Router, Shadcn, TypeScript</p>
                </div>
                <!-- column 2: backend & db -->
                <div class="skill-block">
                    <h3><i class="fa-solid fa-database"></i> Backend & DB</h3>
                    <div class="skill-icons">
                        <img src="https://skillicons.dev/icons?i=nodejs,express,mongodb,postgres,prisma,firebase" alt="backend icons">
                        <span class="custom-icon"><i class="fa-solid fa-lock"></i> Better‑Auth</span>
                        <span class="custom-icon"><i class="fa-solid fa-key"></i> JWT</span>
                    </div>
                    <p style="margin-top: 1.2rem; color:#b1bac4;"><i class="fa-regular fa-circle-check text-neon"></i> Prisma ORM, PostgreSQL, MongoDB, Firebase Auth & Better‑Auth</p>
                </div>
            </div>

            <!-- extra row for auth / deployment expertise (show new auth) -->
            <div style="display: flex; flex-wrap: wrap; gap: 1rem; margin: 1.5rem 0;">
                <div class="skill-block" style="flex:1; min-width:200px;">
                    <h3 style="font-size:1.3rem;">🔐 Authentication</h3>
                    <div class="skill-icons">
                        <span class="custom-icon"><i class="fa-brands fa-google"></i> Firebase Auth</span>
                        <span class="custom-icon"><i class="fa-solid fa-lock-keyhole"></i> Better‑Auth</span>
                        <span class="custom-icon"><i class="fa-solid fa-shield"></i> JWT</span>
                        <span class="custom-icon"><i class="fa-brands fa-github"></i> OAuth</span>
                    </div>
                </div>
                <div class="skill-block" style="flex:1; min-width:200px;">
                    <h3 style="font-size:1.3rem;">🌍 Deploy & tools</h3>
                    <div class="skill-icons">
                        <img src="https://skillicons.dev/icons?i=vercel,netlify,git,postman" alt="deploy">
                        <span class="custom-icon"><i class="fa-solid fa-fire"></i> Firebase</span>
                        <span class="custom-icon"><i class="fa-regular fa-window-maximize"></i> Shadcn</span>
                    </div>
                </div>
            </div>

            <!-- currently section (updated) -->
            <div class="section-title"><i class="fa-regular fa-clock"></i> 📌 current focus</div>
            <ul style="display: grid; grid-template-columns: repeat(auto-fit,minmax(240px,1fr)); gap: 1rem; list-style: none;">
                <li style="background:#161b22; border-radius: 20px; padding: 1.2rem;"><i class="fa-solid fa-cart-shopping text-neon"></i> <strong>E‑commerce MERN</strong> + Better‑Auth, Shadcn</li>
                <li style="background:#161b22; border-radius: 20px; padding: 1.2rem;"><i class="fa-brands fa-react text-neon"></i> <strong>Next.js</strong> with Prisma & PostgreSQL</li>
                <li style="background:#161b22; border-radius: 20px; padding: 1.2rem;"><i class="fa-solid fa-cloud text-neon"></i> <strong>Full‑stack deployment</strong> (Vercel + Neon DB)</li>
                <li style="background:#161b22; border-radius: 20px; padding: 1.2rem;"><i class="fa-solid fa-pen-ruler text-neon"></i> <strong>Shadcn/ui</strong> component systems</li>
            </ul>

            <!-- DEPLOYMENT WORKFLOW mermaid (upgraded) -->
            <div class="section-title"><i class="fa-solid fa-diagram-project"></i> 🚀 deploy flow</div>
            <div class="mermaid-box">
                <div class="mermaid">
                    <pre style="font-family: 'Fira Code', monospace; background: #0d1117; color: #ddd;">
<span style="color:#2dba7e;">graph LR</span>
    A[Local Dev] --> B[GitHub]
    B --> C[Vercel]
    B --> D[Netlify]
    B --> E[Firebase Hosting]
    C --> F[Next.js frontend]
    D --> G[static/SPA]
    E --> H[Full‑stack]
    F --> I((Users))
    G --> I
    H --> I
    subgraph backend: [Prisma + PostgreSQL]
        J[(Neon<br/>MongoDB Atlas)]
    end
    F -.-> J
    H -.-> J
                    </pre>
                </div>
                <p style="margin-top:1rem; color: #8b949e;"><i class="fa-regular fa-note-sticky"></i> Better‑Auth integrated, Shadcn UI, Prisma data layer</p>
            </div>

            <!-- github stats (preserved) -->
            <div class="section-title"><i class="fa-solid fa-chart-simple"></i> 📈 insights</div>
            <div class="stats-container">
                <div class="stat-item"><i class="fa-regular fa-star"></i> 200+ stars</div>
                <div class="stat-item"><i class="fa-regular fa-code-fork"></i> 45+ forks</div>
                <div class="stat-item"><i class="fa-regular fa-eye"></i> 1.2k views</div>
            </div>

            <p align="center" style="margin: 2rem 0 1rem;">
                <img width="48%" src="https://github-readme-stats.vercel.app/api?username=Parvez141300&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="stats" />
                <img width="48%" src="https://github-readme-streak-stats.herokuapp.com/?user=Parvez141300&theme=tokyonight&hide_border=true" alt="streak" />
            </p>
            <p align="center">
                <img width="48%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Parvez141300&layout=compact&theme=tokyonight&hide_border=true" alt="top langs" />
                <img width="48%" src="https://github-profile-trophy.vercel.app/?username=Parvez141300&theme=tokyonight&no-frame=true&margin-w=10&row=2&column=4" alt="trophy" />
            </p>

            <!-- profile view counter (from original) -->
            <p align="center">
                <img src="https://komarev.com/ghpvc/?username=Parvez141300&color=blue&style=for-the-badge" alt="views" />
            </p>

            <!-- Extra callout: new skills summary -->
            <hr />
            <div style="display:flex; flex-wrap:wrap; justify-content:space-between; gap:1.2rem; background: #161b22; border-radius: 40px; padding: 1.5rem 2rem;">
                <span><i class="fa-brands fa-js text-neon"></i> TypeScript full‑stack</span>
                <span><i class="fa-solid fa-laptop-code text-neon"></i> Prisma + Postgres</span>
                <span><i class="fa-regular fa-building text-neon"></i> Shadcn/ui</span>
                <span><i class="fa-solid fa-key text-neon"></i> Better‑Auth</span>
                <span><i class="fa-regular fa-gem text-neon"></i> Next.js</span>
            </div>

            <!-- footer (humor) -->
            <div class="profile-footer">
                <i class="fa-regular fa-heart" style="color:#2dba7e;"></i> building with Next, Prisma, Better‑Auth
            </div>
        </div> <!-- content end -->
    </div> <!-- profile-card -->
</body>
</html>
