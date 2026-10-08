<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Teacher's Day Letter for Sir Randy Bello</title>

    <style>
         :root {
            --bg: #071426;
            --surface: #0c203d;
            --surface-2: #102b4f;
            --text: #e9f4ff;
            --muted: #9bb7d6;
            --primary: #4da8ff;
            --secondary: #8bd4ff;
            --accent: #ff719d;
            --border: #26619a;
            --shadow: rgba(0, 0, 0, 0.35);
        }
        
        body.light {
            --bg: #eaf5ff;
            --surface: #ffffff;
            --surface-2: #d7edff;
            --text: #0b2442;
            --muted: #476581;
            --primary: #126bc4;
            --secondary: #4da8ff;
            --accent: #e54879;
            --border: #78b8e8;
            --shadow: rgba(28, 88, 135, 0.2);
        }
        
        * {
            box-sizing: border-box;
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        body {
            margin: 0;
            min-height: 100vh;
            overflow-x: hidden;
            color: var(--text);
            background: linear-gradient(rgba(77, 168, 255, 0.04) 1px, transparent 1px), linear-gradient(90deg, rgba(77, 168, 255, 0.04) 1px, transparent 1px), var(--bg);
            background-size: 24px 24px;
            font-family: "Courier New", monospace;
            transition: background-color 0.5s ease, color 0.5s ease;
        }
        
        body::before,
        body::after {
            content: "";
            position: fixed;
            z-index: -1;
            width: 180px;
            height: 180px;
            opacity: 0.18;
            pointer-events: none;
            background: var(--primary);
            clip-path: polygon( 0 20%, 20% 20%, 20% 0, 80% 0, 80% 20%, 100% 20%, 100% 80%, 80% 80%, 80% 100%, 20% 100%, 20% 80%, 0 80%);
            filter: blur(2px);
        }
        
        body::before {
            top: 8%;
            left: -90px;
        }
        
        body::after {
            right: -90px;
            bottom: 8%;
            background: var(--accent);
        }
        
        button {
            font: inherit;
        }
        
        .page {
            width: min(100% - 32px, 980px);
            margin: 0 auto;
            padding: 28px 0 48px;
        }
        
        .topbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 16px;
            margin-bottom: 42px;
        }
        
        .pixel-label {
            color: var(--secondary);
            font-size: 0.78rem;
            letter-spacing: 0.14em;
            text-transform: uppercase;
        }
        
        .theme-toggle {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            cursor: pointer;
            color: var(--text);
            border: 2px solid var(--border);
            background: var(--surface);
            padding: 9px 13px;
            box-shadow: 4px 4px 0 var(--shadow);
            transition: background 0.35s ease, color 0.35s ease, transform 0.2s ease;
        }
        
        .theme-toggle:hover {
            transform: translate(-2px, -2px);
        }
        
        .theme-toggle:focus-visible,
        .action-button:focus-visible {
            outline: 3px solid var(--accent);
            outline-offset: 4px;
        }
        
        .switch {
            position: relative;
            width: 42px;
            height: 22px;
            background: var(--muted);
            border: 2px solid var(--text);
        }
        
        .switch::after {
            content: "";
            position: absolute;
            top: 2px;
            left: 2px;
            width: 14px;
            height: 14px;
            background: var(--text);
            transition: transform 0.3s ease;
        }
        
        body.light .switch::after {
            transform: translateX(18px);
        }
        
        .hero {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .hero h1 {
            max-width: 760px;
            margin: 14px auto;
            color: var(--text);
            font-size: clamp(2rem, 6vw, 4.8rem);
            line-height: 1.05;
            letter-spacing: -0.06em;
            text-shadow: 5px 5px 0 rgba(77, 168, 255, 0.2);
        }
        
        .hero p {
            max-width: 620px;
            margin: 0 auto;
            color: var(--muted);
            line-height: 1.7;
            font-family: Arial, sans-serif;
        }
        
        .letter-area {
            position: relative;
            display: grid;
            place-items: center;
            min-height: 590px;
        }
        
        .envelope {
            position: relative;
            width: min(100%, 650px);
            min-height: 360px;
            perspective: 1000px;
        }
        
        .envelope-back {
            position: absolute;
            inset: 0;
            background: var(--surface-2);
            border: 4px solid var(--border);
            box-shadow: 10px 10px 0 var(--shadow);
            clip-path: polygon(0 0, 50% 48%, 100% 0, 100% 100%, 0 100%);
        }
        
        .envelope-front {
            position: absolute;
            inset: 0;
            z-index: 3;
            background: var(--surface);
            border: 4px solid var(--border);
            clip-path: polygon(0 0, 50% 53%, 100% 0, 100% 100%, 0 100%);
            transition: opacity 0.55s ease, transform 0.75s ease;
        }
        
        .flap {
            position: absolute;
            z-index: 4;
            top: 0;
            left: 0;
            width: 100%;
            height: 55%;
            background: var(--surface-2);
            border: 4px solid var(--border);
            transform-origin: top center;
            clip-path: polygon(0 0, 100% 0, 50% 100%);
            transition: transform 0.85s cubic-bezier(0.2, 0.8, 0.2, 1), z-index 0.1s 0.4s;
        }
        
        .seal {
            position: absolute;
            z-index: 5;
            top: 44%;
            left: 50%;
            width: 64px;
            height: 64px;
            transform: translate(-50%, -50%);
            display: grid;
            place-items: center;
            color: white;
            background: var(--accent);
            border: 4px solid var(--surface);
            box-shadow: 0 0 0 3px var(--accent);
            clip-path: polygon( 25% 0, 75% 0, 75% 10%, 90% 10%, 90% 25%, 100% 25%, 100% 75%, 90% 75%, 90% 90%, 75% 90%, 75% 100%, 25% 100%, 25% 90%, 10% 90%, 10% 75%, 0 75%, 0 25%, 10% 25%, 10% 10%, 25% 10%);
            transition: opacity 0.4s ease, transform 0.5s ease;
        }
        
        .letter {
            position: absolute;
            z-index: 2;
            left: 5%;
            right: 5%;
            top: 24px;
            min-height: 500px;
            padding: clamp(24px, 5vw, 52px);
            color: var(--text);
            background: var(--surface);
            border: 4px solid var(--border);
            box-shadow: 8px 8px 0 var(--shadow);
            opacity: 0;
            transform: translateY(70px) scale(0.96);
            transition: opacity 0.7s ease 0.35s, transform 0.8s cubic-bezier(0.2, 0.8, 0.2, 1) 0.35s;
        }
        
        .letter h2 {
            margin-top: 0;
            color: var(--secondary);
            font-size: clamp(1.4rem, 4vw, 2rem);
        }
        
        .letter p {
            color: var(--text);
            font-family: Georgia, serif;
            font-size: 1.08rem;
            line-height: 1.85;
        }
        
        .signature {
            margin-top: 32px;
            color: var(--accent);
            font-weight: bold;
            line-height: 1.7;
        }
        
        .envelope.open .flap {
            z-index: 1;
            transform: rotateX(180deg);
        }
        
        .envelope.open .envelope-front {
            opacity: 0;
            pointer-events: none;
        }
        
        .envelope.open .seal {
            opacity: 0;
            transform: translate(-50%, -50%) scale(0);
        }
        
        .envelope.open .letter {
            z-index: 6;
            opacity: 1;
            transform: translateY(-105px) scale(1);
        }
        
        .controls {
            position: absolute;
            z-index: 10;
            bottom: -10px;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 12px;
        }
        
        .action-button {
            cursor: pointer;
            padding: 13px 18px;
            color: var(--text);
            background: var(--surface);
            border: 3px solid var(--primary);
            box-shadow: 5px 5px 0 var(--shadow);
            transition: color 0.3s ease, background 0.3s ease, transform 0.2s ease;
        }
        
        .action-button:hover {
            transform: translate(-3px, -3px);
            color: white;
            background: var(--primary);
        }
        
        .hearts {
            position: absolute;
            inset: 0;
            z-index: 8;
            overflow: hidden;
            pointer-events: none;
        }
        
        .heart {
            position: absolute;
            bottom: 30%;
            width: 16px;
            height: 16px;
            opacity: 0;
            background: var(--accent);
            transform: rotate(45deg);
        }
        
        .heart::before,
        .heart::after {
            content: "";
            position: absolute;
            width: 16px;
            height: 16px;
            border-radius: 50%;
            background: inherit;
        }
        
        .heart::before {
            left: -8px;
        }
        
        .heart::after {
            top: -8px;
        }
        
        .heart:nth-child(1) {
            left: 22%;
        }
        
        .heart:nth-child(2) {
            left: 39%;
            transform: rotate(45deg) scale(0.7);
        }
        
        .heart:nth-child(3) {
            left: 58%;
            transform: rotate(45deg) scale(1.3);
        }
        
        .heart:nth-child(4) {
            left: 76%;
            transform: rotate(45deg) scale(0.8);
        }
        
        .envelope.open~.hearts .heart {
            animation: floatHeart 3.4s ease-in-out forwards;
        }
        
        .envelope.open~.hearts .heart:nth-child(2) {
            animation-delay: 0.35s;
        }
        
        .envelope.open~.hearts .heart:nth-child(3) {
            animation-delay: 0.7s;
        }
        
        .envelope.open~.hearts .heart:nth-child(4) {
            animation-delay: 1s;
        }
        
        @keyframes floatHeart {
            0% {
                opacity: 0;
                transform: translateY(0) rotate(45deg) scale(0.5);
            }
            20% {
                opacity: 1;
            }
            100% {
                opacity: 0;
                transform: translateY(-310px) rotate(45deg) scale(1.1);
            }
        }
        
        .footer {
            margin-top: 56px;
            color: var(--muted);
            text-align: center;
            font-size: 0.8rem;
        }
        
        @media (max-width: 620px) {
            .page {
                width: min(100% - 20px, 980px);
                padding-top: 18px;
            }
            .topbar {
                align-items: flex-start;
            }
            .theme-toggle {
                padding: 7px 9px;
                font-size: 0.7rem;
            }
            .letter-area {
                min-height: 640px;
            }
            .envelope {
                min-height: 330px;
            }
            .letter {
                min-height: 570px;
                padding: 25px 20px;
            }
            .letter p {
                font-size: 1rem;
                line-height: 1.7;
            }
            .envelope.open .letter {
                transform: translateY(-80px) scale(1);
            }
            .controls {
                bottom: 8px;
            }
        }
        
        @media (prefers-reduced-motion: reduce) {
            *,
            *::before,
            *::after {
                scroll-behavior: auto !important;
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                transition-duration: 0.01ms !important;
            }
        }
    </style>
</head>

<body>
    <main class="page">
        <header class="topbar">
            <div class="pixel-label">Teacher's Day // 2026</div>

            <button class="theme-toggle" id="themeToggle" type="button" aria-label="Switch between dark mode and light mode" aria-pressed="false">
        <span id="themeText">Light Mode</span>
        <span class="switch" aria-hidden="true"></span>
      </button>
        </header>

        <section class="hero" aria-labelledby="pageTitle">
            <div class="pixel-label">A special message from your students</div>
            <h1 id="pageTitle">Happy Teacher's Day,<br />Sir Randy Bello</h1>
            <p>
                A small interactive letter for the instructor who helps students learn, create, and build with confidence.
            </p>
        </section>

        <section class="letter-area" aria-label="Interactive Teacher's Day letter">
            <div class="envelope" id="envelope">
                <div class="envelope-back"></div>

                <article class="letter" aria-live="polite">
                    <h2>Dear Sir Randy Bello,</h2>

                    <p>
                        Happy Teacher's Day! Thank you for sharing your knowledge, patience, and experience with us as our web development instructor.
                    </p>

                    <p>
                        Your lessons have helped us understand more than just HTML, CSS, and JavaScript. You have encouraged us to solve problems, explore new ideas, and continue learning even when the code does not work on the first try.
                    </p>

                    <p>
                        Thank you for your guidance, support, and dedication. Your encouragement inspires us to keep building, improving, and believing in what we can create.
                    </p>

                    <p>
                        We truly appreciate everything you do for your students.
                    </p>

                    <div class="signature">
                        With gratitude and appreciation,<br /> Your Students
                    </div>
                </article>

                <div class="flap"></div>
                <div class="envelope-front"></div>

                <div class="seal" aria-hidden="true">♥</div>

                <div class="controls">
                    <button class="action-button" id="openButton" type="button">
            Open Letter
          </button>

                    <button class="action-button" id="closeButton" type="button" hidden>
            Close Letter
          </button>
                </div>
            </div>

            <div class="hearts" aria-hidden="true">
                <span class="heart"></span>
                <span class="heart"></span>
                <span class="heart"></span>
                <span class="heart"></span>
            </div>
        </section>

        <footer class="footer">
            Made with appreciation, creativity, and a little bit of code.
        </footer>
    </main>

    <script>
        const envelope = document.getElementById("envelope");
        const openButton = document.getElementById("openButton");
        const closeButton = document.getElementById("closeButton");
        const themeToggle = document.getElementById("themeToggle");
        const themeText = document.getElementById("themeText");

        function openLetter() {
            envelope.classList.add("open");
            openButton.hidden = true;
            closeButton.hidden = false;
        }

        function closeLetter() {
            envelope.classList.remove("open");
            closeButton.hidden = true;
            openButton.hidden = false;
        }

        function toggleTheme() {
            const isLight = document.body.classList.toggle("light");

            themeToggle.setAttribute("aria-pressed", String(isLight));
            themeText.textContent = isLight ? "Dark Mode" : "Light Mode";
        }

        openButton.addEventListener("click", openLetter);
        closeButton.addEventListener("click", closeLetter);
        themeToggle.addEventListener("click", toggleTheme);

        document.addEventListener("keydown", (event) => {
            if (event.key === "Escape" && envelope.classList.contains("open")) {
                closeLetter();
            }
        });
    </script>
</body>

</html>
