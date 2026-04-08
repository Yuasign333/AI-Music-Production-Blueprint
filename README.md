<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Music Production Blueprint</title>
    <style>
        :root {
            --bg-color: #0f172a;
            --text-color: #f8fafc;
            --primary: #ec4899; /* Pink */
            --secondary: #3b82f6; /* Blue */
            --card-bg: #1e293b;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }

        /* --- PAYWALL JOKE SECTION --- */
        #paywall-section {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            text-align: center;
            padding: 20px;
        }

        .meme-box {
            background: var(--card-bg);
            padding: 40px 20px;
            border-radius: 12px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.5);
            border: 2px solid var(--primary);
            max-width: 400px;
            width: 100%;
        }

        .meme-box h1 {
            color: var(--primary);
            margin-bottom: 10px;
        }

        .meme-box p {
            margin-bottom: 30px;
            color: #cbd5e1;
        }

        .pay-btn {
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2rem;
            font-weight: bold;
            border-radius: 8px;
            cursor: pointer;
            width: 100%;
            transition: transform 0.2s, opacity 0.2s;
        }

        .pay-btn:hover {
            opacity: 0.9;
            transform: scale(1.02);
        }

        /* --- BLUEPRINT SECTION --- */
        #blueprint-section {
            display: none; /* Hidden by default */
            animation: fadeIn 1s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
            padding-top: 20px;
        }

        .header h1 {
            background: linear-gradient(90deg, var(--secondary), var(--primary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        .step-card {
            background: var(--card-bg);
            border-radius: 12px;
            padding: 25px;
            margin-bottom: 20px;
            border-left: 5px solid var(--secondary);
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            overflow: hidden;
        }

        .step-card h2 {
            margin-top: 0;
            color: var(--secondary);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .step-card.pink-accent {
            border-left-color: var(--primary);
        }
        .step-card.pink-accent h2 {
            color: var(--primary);
        }

        .tag {
            display: inline-block;
            background: rgba(255, 255, 255, 0.1);
            padding: 5px 10px;
            border-radius: 5px;
            font-family: monospace;
            color: #fbbf24;
            margin-bottom: 10px;
            font-size: 0.9rem;
        }

        ul {
            padding-left: 20px;
        }

        ul li {
            margin-bottom: 10px;
        }

        .cool-img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
            border: 1px solid rgba(255,255,255,0.1);
        }

        /* Mobile Adjustments */
        @media (max-width: 600px) {
            .header h1 { font-size: 2rem; }
            .step-card { padding: 15px; }
            .pay-btn { padding: 12px 20px; font-size: 1.1rem; }
            .cool-img { height: 150px; }
        }
    </style>
</head>
<body>

    <div id="paywall-section">
        <div class="meme-box">
            <h1>🔒 Premium Content</h1>
            <p>You have stumbled upon the Ultimate AI Music Production Masterclass. To reveal the secret workflow, please insert your digital coins.</p>
            <button class="pay-btn" onclick="revealBlueprint()">Pay ₱499 to Access</button>
        </div>
    </div>

    <div id="blueprint-section" class="container">
        <div class="header">
            <h1>AI Music Production Blueprint</h1>
            <p>From Concept to Masterpiece using LLMs, Suno, and BandLab.</p>
        </div>

        <div class="step-card">
            <h2>Phase 1: The Brainstorming (ChatGPT / Gemini)</h2>
            <p>Great music starts with a solid foundation. Use conversational AI to act as your co-writer.</p>
            <ul>
                <li><strong>Lyrics Generation:</strong> Draft your own emotional core, then use an LLM to refine the rhyming scheme, syllable count, and song structure (Verse, Pre-Chorus, Chorus, Bridge).</li>
                <li><strong>Creative Direction:</strong> Tell the AI your concept (e.g., "A bittersweet blue and pink aesthetic") to generate metaphors and imagery for your lyrics.</li>
            </ul>
        </div>

        <div class="step-card pink-accent">
            <h2>Phase 2: Prompt Engineering (LLM Control Technique)</h2>
            <p>Suno needs precise instructions. Use Gemini or ChatGPT to structure the perfect "Style Prompt" to control the genre, instruments, and vocal tone.</p>
            <ul>
                <li><strong>Meta Tags:</strong> Instruct your LLM to create detailed tags like <span class="tag">[Vocal Style: Alissa Ace, Cutesy]</span> and <span class="tag">[Arrangement: E Major, Bedpop]</span>.</li>
                <li><strong>Timestamping:</strong> Use the LLM to map out the progression based on a reference audio (e.g., "0:00 Acoustic -> 0:21 Beat drops -> 0:41 Full band").</li>
                <li><strong>Consistency:</strong> The LLM helps ensure your prompt fits within Suno's character limits while keeping the most impactful keywords intact.</li>
            </ul>
        </div>

        <div class="step-card">
            <img src="https://images.unsplash.com/photo-1598488035139-bdbb2231ce04?w=800&q=80" alt="Audio Referencing" class="cool-img">
            <h2>Phase 3: Advanced Audio Referencing (Suno Feature)</h2>
            <p>Don't just type prompts—use actual audio to guide the AI! Upload a video or voice recording to anchor the melody and key (like E Major).</p>
            <ul>
                <li><strong>The 1-Minute Free Trick:</strong> On the Free tier, you can upload up to 1 minute of audio. Record yourself humming the melody, playing a guitar riff, or upload a screen recording of your beat. Suno will extract the vibe and continue the song from there.</li>
                <li><strong>Pro Tier "Studio Transformation":</strong> If you have a Pro account, you can upload your *entire* raw song. Sing into your phone while strumming a guitar, and Suno can transform it into a massive, multi-instrumental studio track while keeping your original structure!</li>
                <li><strong>Voice Transformation:</strong> Want the AI to sound like you? Upload your raw vocal memo as a reference, then use prompt tags like <span class="tag">[Vocal Style: Intimate, breathy, NO BELTING]</span> to force the AI to mimic your original voice and transform it into your desired voice.</li>
            </ul>
        </div>

        <div class="step-card pink-accent">
            <h2>Phase 4: Generation & Iteration (Suno AI)</h2>
            <p>Where the magic happens. Combine your audio reference, prompt, and lyrics.</p>
            <ul>
                <li><strong>Input:</strong> Put your structured lyrics in the lyrics box and your engineered prompt in the "Style of Music" box.</li>
                <li><strong>Iteration:</strong> Generate multiple versions. Listen for the closest match to your desired melody.</li>
                <li><strong>Extension:</strong> If the song ends prematurely or you need a specific outro, use Suno's "Extend" feature from the best timestamp.</li>
            </ul>
        </div>

        <div class="step-card">
            <img src="https://images.unsplash.com/photo-1598653222000-6b7b7a552625?w=800&q=80" alt="Post Production" class="cool-img">
            <h2>Phase 5: Post-Production (BandLab)</h2>
            <p>Take the raw Suno audio and turn it into a professional, polished track.</p>
            <ul>
                <li><strong>AI Splitter:</strong> Import the Suno audio into BandLab and use the "Splitter" tool to separate Vocals, Bass, Drums, and Others.</li>
                <li><strong>Vocal Mixing:</strong> Add EQ (cut the muddy lows), De-Esser, and Reverb/Delay to make the vocals shine.</li>
                <li><strong>Instrument Control:</strong> Lower the volume of harsh instruments, or boost the drums if they feel too weak in the original Suno file.</li>
                <li><strong>Manual Additions:</strong> Record your own vocal ad-libs over it, or add manual MIDI instruments (like extra piano or synths) to fill out the sound.</li>
            </ul>
        </div>
        
        <div class="header" style="margin-top: 50px;">
            <p><em>Made by Yuan</em></p>
        </div>
    </div>

    <script>
        function revealBlueprint() {
            // The Joke Alert
            alert("SIKE! 😂 Joke lang boss! \n\nWala itong bayad. Knowledge should be free! Welcome to the Ultimate AI Music Blueprint.");
            
            // Hide the paywall
            document.getElementById('paywall-section').style.display = 'none';
            
            // Show the blueprint
            document.getElementById('blueprint-section').style.display = 'block';
            
            // Scroll to top just in case
            window.scrollTo(0,0);
        }
    </script>
</body>
</html>
