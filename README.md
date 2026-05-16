<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JARVIS // Core System</title>
    <link rel="stylesheet" href="style.css">
    <!-- Google Fonts for High-Tech look -->
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Share+Tech+Mono&display=swap" rel="stylesheet">
</head>
<body>

    <!-- 1. AI BOOT-UP LOADING SCREEN -->
    <div id="loader">
        <div class="arc-reactor"></div>
        <div class="load-text">INITIALIZING JARVIS SYSTEM...</div>
        <div class="progress-bar"><div class="progress-fill"></div></div>
    </div>

    <!-- 2. MAIN SYSTEM INTERFACE -->
    <div id="main-interface" class="hidden">
        <!-- Header / Status Bar -->
        <header>
            <div class="system-title">JARVIS // CORE_v3.0</div>
            <div class="system-status">SYSTEM STATUS: <span class="online">ONLINE</span></div>
        </header>

        <!-- Main Dashboard Container -->
        <main class="dashboard">
            
            <!-- Left Panel: Profile / Welcome -->
            <section class="panel profile-panel">
                <div class="panel-header">USER PROFILE</div>
                <div class="panel-body">
                    <p class="matrix-text">> USER: <span class="highlight">ANWARULLAH</span></p>
                    <p class="matrix-text">> ACCESS_LEVEL: <span class="highlight">ADMINISTRATOR</span></p>
                    <p class="matrix-text">> REGION: <span class="highlight">KASHMIR_PK</span></p>
                </div>
            </section>

            <!-- Center Panel: Main AI Console -->
            <section class="panel console-panel">
                <div class="panel-header">CENTRAL COMMAND CONSOLE</div>
                <div class="panel-body console-screen">
                    <div class="terminal-output">
                        <p class="line yellow">> Accessing global servers... Done.</p>
                        <p class="line">> System Diagnostics: 100% Operational.</p>
                        <p class="line cyan">> Welcome back, sir. All projects are ready for deployment.</p>
                    </div>
                </div>
            </section>

            <!-- Right Panel: Active Projects -->
            <section class="panel projects-panel">
                <div class="panel-header">ACTIVE MISSIONS</div>
                <div class="panel-body project-list">
                    <div class="project-card">
                        <span class="proj-title">PROJECT_STATPULSE</span>
                        <span class="proj-status">CINEMATIC_DOCS</span>
                    </div>
                    <div class="project-card">
                        <span class="proj-title">WEB_CORE_INTERFACE</span>
                        <span class="proj-status">STARK_LEVEL_UI</span>
                    </div>
                </div>
            </section>

        </main>

        <!-- Footer / Action Area -->
        <footer>
            <div class="footer-note">STARK INDUSTRIES // SECURE INTERFACE</div>
            <button class="action-btn" onclick="systemAlert()">ENGAGE PROTOCOL</button>
        </footer>
    </div>

    <!-- Interactive Audio & Boot Script -->
    <script>
        // Smooth Boot-up Sequence
        window.addEventListener('DOMContentLoaded', () => {
            setTimeout(() => {
                const loader = document.getElementById('loader');
                const mainUI = document.getElementById('main-interface');
                
                loader.style.opacity = '0';
                loader.style.transition = 'opacity 0.8s ease';
                
                setTimeout(() => {
                    loader.style.display = 'none';
                    mainUI.classList.remove('hidden');
                    mainUI.style.opacity = '0';
                    setTimeout(() => {
                        mainUI.style.opacity = '1';
                        mainUI.style.transition = 'opacity 1.5s ease';
                    }, 50);
                }, 800);
            }, 3500); // 3.5 seconds boot animation
        });

        function systemAlert() {
            alert("SYSTEM WARNING: Stark Interface Online. Protocol 11 Engaged.");
        }
    </script>
</body>
</html>
