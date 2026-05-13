# buscadores <!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portal de Buscadores</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        .container {
            max-width: 1000px;
            width: 100%;
        }

        .header {
            text-align: center;
            color: white;
            margin-bottom: 50px;
        }

        .header h1 {
            font-size: 3em;
            font-weight: 700;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }

        .header p {
            font-size: 1.2em;
            opacity: 0.9;
            font-weight: 300;
        }

        .buscadores-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin-bottom: 40px;
        }

        .buscador-card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }

        .buscador-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s ease;
        }

        .buscador-card:hover::before {
            left: 100%;
        }

        .buscador-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
        }

        .buscador-icon {
            font-size: 3.5em;
            margin-bottom: 15px;
            display: block;
        }

        .buscador-card h2 {
            font-size: 1.8em;
            color: #333;
            margin-bottom: 10px;
            font-weight: 600;
        }

        .buscador-card p {
            color: #666;
            font-size: 0.95em;
            margin-bottom: 20px;
            line-height: 1.5;
        }

        .buscador-card a {
            display: inline-block;
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            padding: 12px 30px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .buscador-card a:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(102, 126, 234, 0.6);
        }

        .buscador-card a:active {
            transform: scale(0.98);
        }

        .footer {
            text-align: center;
            color: rgba(255, 255, 255, 0.8);
            font-size: 0.9em;
            margin-top: 40px;
        }

        @media (max-width: 768px) {
            .header h1 {
                font-size: 2em;
            }

            .header p {
                font-size: 1em;
            }

            .buscadores-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }

            .buscador-card {
                padding: 25px;
            }

            .buscador-icon {
                font-size: 2.8em;
            }

            .buscador-card h2 {
                font-size: 1.5em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>🔍 Buscadores</h1>
            <p>Accede a los principales motores de búsqueda</p>
        </div>

        <div class="buscadores-grid">
            <!-- Google -->
            <div class="buscador-card">
                <span class="buscador-icon">🔵</span>
                <h2>Google</h2>
                <p>El buscador más popular del mundo</p>
                <a href="https://www.google.com" target="_blank">Ir a Google</a>
            </div>

            <!-- Bing -->
            <div class="buscador-card">
                <span class="buscador-icon">🔷</span>
                <h2>Bing</h2>
                <p>Buscador de Microsoft con imágenes destacadas</p>
                <a href="https://www.bing.com" target="_blank">Ir a Bing</a>
            </div>

            <!-- DuckDuckGo -->
            <div class="buscador-card">
                <span class="buscador-icon">🦆</span>
                <h2>DuckDuckGo</h2>
                <p>Privacidad garantizada en tus búsquedas</p>
                <a href="https://duckduckgo.com" target="_blank">Ir a DuckDuckGo</a>
            </div>

            <!-- Yahoo -->
            <div class="buscador-card">
                <span class="buscador-icon">💜</span>
                <h2>Yahoo</h2>
                <p>Portal de búsqueda con noticias integradas</p>
                <a href="https://www.yahoo.com" target="_blank">Ir a Yahoo</a>
            </div>

            <!-- Ecosia -->
            <div class="buscador-card">
                <span class="buscador-icon">🌱</span>
                <h2>Ecosia</h2>
                <p>Búsqueda sostenible que planta árboles</p>
                <a href="https://www.ecosia.org" target="_blank">Ir a Ecosia</a>
            </div>

            <!-- Safari -->
            <div class="buscador-card">
                <span class="buscador-icon">🧭</span>
                <h2>Safari</h2>
                <p>Navegador Apple integrado</p>
                <a href="https://www.apple.com/safari" target="_blank">Ir a Safari</a>
            </div>
        </div>

        <div class="footer">
            <p>© 2026 Portal de Buscadores - Diseñado con elegancia</p>
        </div>
    </div>
</body>
</html>