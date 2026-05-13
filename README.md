# kanda.github.io
Happy Graduate!
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Graduation Congratulations</title>
    <link href="[fonts.googleapis.com](https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Montserrat:wght@300;400;500&display=swap)" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
            padding: 20px;
            font-family: 'Montserrat', sans-serif;
        }

        .card {
            background: linear-gradient(145deg, #ffffff 0%, #f8f9fa 100%);
            border-radius: 20px;
            padding: 50px 40px;
            max-width: 600px;
            width: 100%;
            box-shadow: 
                0 25px 50px rgba(0, 0, 0, 0.3),
                0 0 100px rgba(212, 175, 55, 0.2);
            position: relative;
            overflow: hidden;
        }

        .card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 8px;
            background: linear-gradient(90deg, #d4af37, #f4d03f, #d4af37);
        }

        .decoration {
            position: absolute;
            font-size: 120px;
            opacity: 0.05;
            top: -20px;
            right: -10px;
        }

        .cap-icon {
            text-align: center;
            font-size: 80px;
            margin-bottom: 20px;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .header {
            text-align: center;
            margin-bottom: 30px;
        }

        .header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: #1a1a2e;
            margin-bottom: 10px;
            letter-spacing: 2px;
        }

        .header .subtitle {
            font-size: 1.1rem;
            color: #d4af37;
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 3px;
        }

        .divider {
            width: 100px;
            height: 3px;
            background: linear-gradient(90deg, transparent, #d4af37, transparent);
            margin: 25px auto;
        }

        .graduate-name {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            color: #0f3460;
            margin: 20px 0;
            font-weight: 700;
        }

        .degree {
            text-align: center;
            font-size: 1rem;
            color: #555;
            margin-bottom: 30px;
            font-weight: 300;
        }

        .message {
            text-align: center;
            line-height: 1.8;
            color: #444;
            font-size: 1.05rem;
            padding: 0 20px;
            margin-bottom: 30px;
        }

        .date {
            text-align: center;
            color: #888;
            font-size: 0.95rem;
            margin-top: 30px;
        }

        .signature {
            text-align: center;
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid #eee;
        }

        .signature .from {
            font-style: italic;
            color: #666;
            margin-bottom: 5px;
        }

        .signature .name {
            font-family: 'Playfair Display', serif;
            font-size: 1.3rem;
            color: #1a1a2e;
        }

        .confetti {
            position: fixed;
            width: 10px;
            height: 10px;
            top: -10px;
            animation: fall linear forwards;
        }

        @keyframes fall {
            to {
                transform: translateY(100vh) rotate(720deg);
            }
        }

        .stars {
            text-align: center;
            font-size: 1.5rem;
            letter-spacing: 10px;
            margin: 20px 0;
        }

        @media (max-width: 480px) {
            .card {
                padding: 30px 20px;
            }
            .header h1 {
                font-size: 1.8rem;
            }
            .graduate-name {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="decoration">🎓</div>
        
        <div class="cap-icon">🎓</div>
        
        <div class="header">
            <p class="subtitle">Class of 2025</p>
            <h1>Congratulations!</h1>
        </div>
        
        <div class="divider"></div>
        
        <p class="graduate-name">John Doe</p>
        <p class="degree">Bachelor of Science in Computer Science</p>
        
        <div class="stars">⭐ ⭐ ⭐</div>
        
        <p class="message">
            Your hard work, dedication, and perseverance have brought you to this 
            incredible milestone. As you step into the next chapter of your life, 
            remember that this achievement is just the beginning of an amazing journey ahead.
            <br><br>
            May your future be as bright as your dreams!
        </p>
        
        <p class="date">May 15, 2025</p>
        
        <div class="signature">
            <p class="from">With love and pride,</p>
            <p class="name">Your Family & Friends</p>
        </div>
    </div>

    <script>
        // Confetti animation
        function createConfetti() {
            const colors = ['#d4af37', '#f4d03f', '#0f3460', '#e74c3c', '#2ecc71', '#9b59b6'];
            
            for (let i = 0; i < 50; i++) {
                setTimeout(() => {
                    const confetti = document.createElement('div');
                    confetti.className = 'confetti';
                    confetti.style.left = Math.random() * 100 + 'vw';
                    confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
                    confetti.style.borderRadius = Math.random() > 0.5 ? '50%' : '0';
                    confetti.style.width = Math.random() * 10 + 5 + 'px';
                    confetti.style.height = confetti.style.width;
                    confetti.style.animationDuration = Math.random() * 3 + 2 + 's';
                    document.body.appendChild(confetti);
                    
                    setTimeout(() => confetti.remove(), 5000);
                }, i * 100);
            }
        }

        // Trigger confetti on page load
        window.addEventListener('load', createConfetti);

        // Optional: Click to replay confetti
        document.querySelector('.card').addEventListener('click', createConfetti);
    </script>
</body>
</html>
