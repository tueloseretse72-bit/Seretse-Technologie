<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Seretse Global Innovation Hub | Secure Learning Framework</title>
    <style>
        /* ==========================================================================
           COMPREHENSIVE HIGH-ACCESSIBILITY GLOBAL IDENTITY STYLESHEET (style.css)
           ========================================================================== */
        :root {
            --bg-dark: #0b0f19;
            --card-dark: #1e293b;
            --accent-blue: #3b82f6;
            --accent-green: #10b981;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
            --risk-weak: #ef4444;
            --risk-medium: #f59e0b;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            line-height: 1.7;
        }

        /* Top Protected Header */
        header {
            background-color: rgba(11, 15, 25, 0.95);
            border-bottom: 1px solid #334155;
            padding: 1.2rem 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        header .logo {
            font-size: 1.4rem;
            font-weight: 800;
            letter-spacing: -0.5px;
        }

        header .logo span {
            color: var(--accent-blue);
        }

        nav ul {
            display: flex;
            list-style: none;
            align-items: center;
        }

        nav ul li a {
            color: var(--text-muted);
            text-decoration: none;
            margin-left: 2rem;
            font-size: 0.95rem;
            transition: color 0.2s ease;
        }

        nav ul li a:hover {
            color: var(--text-main);
        }

        .nav-btn {
            background-color: var(--accent-blue);
            color: white !important;
            padding: 0.5rem 1.2rem;
            border-radius: 6px;
            border: none;
            font-weight: 600;
            cursor: pointer;
            margin-left: 2rem;
            transition: background-color 0.2s ease;
        }

        /* Hero Graphic Space */
        .hero-secure {
            background: linear-gradient(rgba(11, 15, 25, 0.8), rgba(11, 15, 25, 0.95)), url('https://unsplash.com') no-repeat center center/cover;
            min-height: 65vh;
            display: flex;
            align-items: center;
            text-align: center;
            padding: 0 2rem;
        }

        .hero-overlay {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero-overlay h1 {
            font-size: 3.2rem;
            line-height: 1.2;
            margin-bottom: 1.5rem;
            font-weight: 800;
        }

        .hero-overlay p {
            font-size: 1.25rem;
            color: var(--text-muted);
            margin-bottom: 2.5rem;
        }

        /* Buttons & Badges */
        .cta-group {
            display: flex;
            gap: 1rem;
            justify-content: center;
        }

        .btn {
            padding: 0.8rem 2rem;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1rem;
            transition: all 0.2s ease;
            display: inline-block;
        }

        .btn-primary { background-color: var(--accent-blue); color: white; border: none; cursor: pointer; }
        .btn-primary:hover { background-color: #2563eb; }
        .btn-secondary { border: 1px solid #475569; color: var(--text-main); }
        .btn-secondary:hover { background-color: rgba(255,255,255,0.05); }
        .btn-secure { background-color: var(--accent-green); color: white; width: 100%; border: none; cursor: pointer; padding: 0.85rem; font-size: 1rem; border-radius: 6px; font-weight: 600;}
        .btn-secure:hover { background-color: #059669; }

        .badge {
            background-color: rgba(59, 130, 246, 0.15);
            color: var(--accent-blue);
            padding: 0.25rem 0.75rem;
            border-radius: 30px;
            font-size: 0.75rem;
            font-weight: 700;
            text-transform: uppercase;
        }

        /* Sections and Pillar Layouts */
        .pillars-section, .tracks-section, .sandbox-section, .dashboard-panel {
            padding: 5rem 8%;
        }

        h2 {
            font-size: 2.2rem;
            text-align: center;
            margin-bottom: 3rem;
        }

        .pillars-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .pillar-card {
            background-color: var(--card-dark);
            border: 1px solid #334155;
            padding: 2.5rem;
            border-radius: 12px;
            transition: transform 0.2s ease;
        }

        .pillar-card:hover { transform: translateY(-4px); }
        .pillar-card .icon { font-size: 2.5rem; margin-bottom: 1rem; }
        .pillar-card h3 { margin-bottom: 0.8rem; font-size: 1.3rem; }
        .pillar-card p { color: var(--text-muted); }

        /* Dynamic Learning Tracks Rows */
        .tracks-container {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
            max-width: 900px;
            margin: 0 auto;
        }

        .track-row {
            background-color: var(--card-dark);
            border-left: 4px solid var(--accent-blue);
            padding: 2rem;
            border-radius: 0 12px 12px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 1.5rem;
        }

        .track-info h3 { margin: 0.5rem 0; font-size: 1.4rem; }
        .track-info p { color: var(--text-muted); font-size: 0.95rem; }

        .action-btn {
            background-color: transparent;
            border: 1px solid var(--accent-blue);
            color: var(--accent-blue);
            padding: 0.6rem 1.5rem;
            border-radius: 6px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.2s;
        }

        .action-btn:hover { background-color: var(--accent-blue); color: white; }

        /* Real-Time Dashboard Analytics */
        .dashboard-panel { background: #111827; }
        .dashboard-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 1.5rem;
            max-width: 900px;
            margin: 0 auto;
        }
        .dash-card {
            background: var(--card-dark);
            padding: 2rem;
            border-radius: 12px;
            border: 1px solid #334155;
            text-align: center;
        }
        .dash-card h4 { color: var(--text-muted); margin-bottom: 0.5rem; font-size: 0.9rem; text-transform: uppercase; }
        .metric-value { font-size: 1.8rem; font-weight: 700; color: var(--accent-blue); }

        /* Secure Sandbox Form layout */
        .form-wrapper {
            max-width: 600px;
            margin: 0 auto;
            background-color: var(--card-dark);
            padding: 3rem;
            border-radius: 16px;
            border: 1px solid #334155;
        }
        .form-wrapper h2, .form-wrapper p { text-align: left; }
        .form-wrapper p { color: var(--text-muted); margin-bottom: 2rem; }
        .form-group { margin-bottom: 1.5rem; text-align: left; }
        .form-group label { display: block; margin-bottom: 0.5rem; font-size: 0.9rem; color: var(--text-muted); }
        .secure-form select, .secure-form textarea {
            width: 100%; padding: 0.85rem; background-color: var(--bg-dark);
            border: 1px solid #475569; border-radius: 6px; color: white; font-size: 1rem;
        }

        /* Cinematic Animation Modals Overlay */
        .modal-overlay {
            position: fixed; top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(11, 15, 25, 0); backdrop-filter: blur(0px);
            display: flex; align-items: center; justify-content: center;
            z-index: 2000; opacity: 0; pointer-events: none;
            transition: opacity 0.4s cubic-bezier(0.16, 1, 0.3, 1), backdrop-filter 0.4s cubic-bezier(0.16, 1, 0.3, 1);
            padding: 1rem;
        }
        .modal-box {
            background: var(--card-dark); border: 1px solid #334155; padding: 2.5rem;
            border-radius: 16px; max-width: 500px; width: 100%;
            transform: translateY(30px) scale(0.95); transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1);
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.6);
        }
        .modal-overlay.modal-active { opacity: 1; pointer-events: all; background: rgba(11, 15, 25, 0.85); backdrop-filter: blur(8px); }
        .modal-overlay.modal-active .modal-box { transform: translateY(0) scale(1); }
        
        .modal-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 1.5rem; border-bottom: 1px solid #334155; padding-bottom: 0.75rem; }
        .close-btn { background: transparent; border: none; color: var(--text-muted); font-size: 1.75rem; cursor: pointer; }
        .close-btn:hover { color: white; }
        .hidden { display: none !important; }

        /* Security Password Strength Bars */
        .strength-bar-container { background: #334155; height: 6px; border-radius: 4px; margin-top: 0.5rem; overflow: hidden; }
