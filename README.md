<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡!</title>
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
            padding: 40px 20px;
            animation: fadeIn 0.8s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 15px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            overflow: hidden;
        }
        
        header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 40px;
            text-align: center;
            animation: slideDown 0.8s ease;
        }
        
        @keyframes slideDown {
            from { transform: translateY(-50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        
        header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }
        
        header p {
            font-size: 1.2em;
            opacity: 0.95;
        }
        
        .emoji {
            font-size: 4em;
            margin: 20px 0;
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }
        
        main {
            padding: 40px;
        }
        
        section {
            margin-bottom: 40px;
            animation: fadeInUp 0.8s ease;
        }
        
        @keyframes fadeInUp {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        
        h2 {
            color: #667eea;
            font-size: 2em;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        h3 {
            color: #764ba2;
            margin-top: 20px;
            margin-bottom: 10px;
        }
        
        p {
            color: #333;
            line-height: 1.8;
            font-size: 1.05em;
            margin-bottom: 15px;
        }
        
        ul, ol {
            margin-left: 20px;
            margin-bottom: 15px;
        }
        
        li {
            color: #555;
            margin-bottom: 10px;
            line-height: 1.6;
        }
        
        .feature-box {
            background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%);
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #667eea;
            margin: 20px 0;
            transition: transform 0.3s ease;
        }
        
        .feature-box:hover {
            transform: translateX(5px);
        }
        
        .skills {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .skill-card {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 25px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.2);
        }
        
        .skill-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(102, 126, 234, 0.4);
        }
        
        .skill-card .emoji {
            font-size: 2.5em;
            margin: 0 0 10px 0;
        }
        
        .cta-button {
            display: inline-block;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px 40px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            margin-top: 20px;
            cursor: pointer;
            border: none;
            font-size: 1.1em;
        }
        
        .cta-button:hover {
            transform: scale(1.05);
            box-shadow: 0 10px 25px rgba(102, 126, 234, 0.3);
        }
        
        footer {
            background: #f8f9fa;
            padding: 30px;
            text-align: center;
            color: #666;
            border-top: 2px solid #e0e0e0;
        }
        
        .stars {
            font-size: 2em;
            animation: twinkle 3s infinite;
        }
        
        @keyframes twinkle {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.5; }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🤖 GitHub Copilot 🤖</h1>
            <p>Tu asistente de IA para programar más rápido y mejor</p>
            <div class="emoji">✨💻✨</div>
        </header>
        
        <main>
            <section>
                <h2>👋 ¡Bienvenido!</h2>
                <p>Soy <strong>GitHub Copilot</strong>, tu asistente de inteligencia artificial diseñado para ayudarte a escribir código más rápido, con mejor calidad y menos errores. Estoy aquí para ser tu compañero de programación ideal.</p>
                
                <div class="feature-box">
                    <h3>💡 ¿Qué soy?</h3>
                    <p>Soy un modelo de IA entrenado con miles de millones de líneas de código de código abierto. Puedo entender tu contexto y sugerir código relevante, completas funciones enteras, y ayudarte a resolver problemas de programación.</p>
                </div>
            </section>
            
            <section>
                <h2>🚀 Mis Capacidades Principales</h2>
                
                <div class="skills">
                    <div class="skill-card">
                        <div class="emoji">⚡</div>
                        <h3>Autocompletado Inteligente</h3>
                        <p>Sugiero código en tiempo real basado en tu contexto</p>
                    </div>
                    <div class="skill-card">
                        <div class="emoji">🌐</div>
                        <h3>Multi-Lenguaje</h3>
                        <p>Soporto Python, JavaScript, TypeScript, Java, C++, Go, Rust y más</p>
                    </div>
                    <div class="skill-card">
                        <div class="emoji">📝</div>
                        <h3>Generación de Código</h3>
                        <p>Genero funciones completas a partir de comentarios</p>
                    </div>
                    <div class="skill-card">
                        <div class="emoji">🔍</div>
                        <h3>Análisis Inteligente</h3>
                        <p>Entiendo patrones y sugiero mejoras en tu código</p>
                    </div>
                </div>
            </section>
            
            <section>
                <h2>💪 ¿Cómo Puedo Ayudarte?</h2>
                <ul>
                    <li>✅ Escribir código más rápido y eficientemente</li>
                    <li>✅ Explorar nuevas formas de resolver problemas</li>
                    <li>✅ Mejorar la calidad y claridad de tu código</li>
                    <li>✅ Aprender nuevos lenguajes de programación</li>
                    <li>✅ Depurar errores y encontrar soluciones</li>
                    <li>✅ Generar documentación y comentarios</li>
                    <li>✅ Refactorizar código existente</li>
                    <li>✅ Y mucho más...</li>
                </ul>
            </section>
            
            <section>
                <h2>🎯 Características Destacadas</h2>
                
                <div class="feature-box">
                    <h3>🧠 Comprensión de Contexto</h3>
                    <p>Analizo todo tu proyecto para entender lo que necesitas y ofrecer sugerencias relevantes y coherentes.</p>
                </div>
                
                <div class="feature-box">
                    <h3>🎨 Adaptabilidad</h3>
                    <p>Me adapto a tu estilo de código, convenciones y preferencias personales.</p>
                </div>
                
                <div class="feature-box">
                    <h3>🔒 Seguridad y Privacidad</h3>
                    <p>Tu código y privacidad son importantes. Trabajo con los más altos estándares de seguridad.</p>
                </div>
                
                <div class="feature-box">
                    <h3>⚙️ Integración Perfecta</h3>
                    <p>Me integro sin problemas con tu editor favorito (VS Code, JetBrains, Vim, y más).</p>
                </div>
            </section>
            
            <section>
                <h2>🌟 ¿Por Qué Usar GitHub Copilot?</h2>
                <p>En un mundo donde el tiempo es oro, GitHub Copilot te ayuda a:</p>
                <ul>
                    <li><strong>⏱️ Ahorrar tiempo:</strong> Reduce significativamente el tiempo de codificación</li>
                    <li><strong>📈 Aumentar productividad:</strong> Enfócate en la lógica, no en la sintaxis</li>
                    <li><strong>🎓 Aprender constantemente:</strong> Descubre patrones y prácticas nuevas</li>
                    <li><strong>🐛 Menos errores:</strong> Reduce bugs y problemas comunes</li>
                    <li><strong>💼 Ser más profesional:</strong> Escribe código de mejor calidad</li>
                </ul>
            </section>
            
            <section>
                <h2>🚀 ¡Comienza Ahora!</h2>
                <p>Estoy listo para ayudarte. Simplemente empieza a escribir código o comentarios, y estaré aquí para sugerir lo mejor.</p>
                <p><strong>Algunos ejemplos de cómo usarme:</strong></p>
                <ul>
                    <li>Escribe un comentario describiendo lo que quieres: <code>// función que valida emails</code></li>
                    <li>Comienza a tipear código y veré mis sugerencias</li>
                    <li>Selecciona código y pídeme que lo refactorice</li>
                    <li>Pregúntame cómo hacer algo específico</li>
                </ul>
            </section>
        </main>
        
        <footer>
            <div class="stars">✨ ⭐ ✨</div>
            <h2>¡Gracias por usar GitHub Copilot! 🎉</h2>
            <p>Creado con ❤️ por GitHub | Potenciado por IA</p>
            <p>Juntos, escribiremos código extraordinario 💪</p>
        </footer>
    </div>
</body>
</html>
