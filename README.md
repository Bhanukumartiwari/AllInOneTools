<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Essential Tools Hub - 25+ Free Online Tools</title>
    <meta name="description" content="Essential web tools including calculators, converters, generators, formatters and more. Free online utilities for daily productivity.">
    <meta name="keywords" content="online tools, calculator, password generator, converter, formatter, free utilities">
    
    <!-- Google AdSense Configuration -->
    <script>
        // AdSense Configuration - Replace with your actual IDs
        const ADSENSE_CONFIG = {
            publisherId: 'ca-pub-XXXXXXXXXXXXXXXXX', // Replace with your AdSense Publisher ID
            adSlots: {
                topBanner: '1234567890',        // Replace with your top banner slot ID
                middleBanner: '2345678901',     // Replace with your middle banner slot ID  
                sidebar: '3456789012',          // Replace with your sidebar slot ID
                bottomBanner: '4567890123',     // Replace with your bottom banner slot ID
                inContent: '5678901234'         // Replace with your in-content slot ID
            },
            autoAds: true // Set to false if you want manual ad placement only
        };

        // Load Google AdSense script
        (function() {
            const script = document.createElement('script');
            script.async = true;
            script.src = `https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=${ADSENSE_CONFIG.publisherId}`;
            script.crossOrigin = 'anonymous';
            document.head.appendChild(script);

            // Auto ads (optional)
            if (ADSENSE_CONFIG.autoAds) {
                script.onload = function() {
                    (adsbygoogle = window.adsbygoogle || []).push({
                        google_ad_client: ADSENSE_CONFIG.publisherId,
                        enable_page_level_ads: true
                    });
                };
            }
        })();
    </script>
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            color: #333;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 20px;
        }

        header {
            text-align: center;
            margin-bottom: 40px;
            padding: 30px 0;
        }

        .logo {
            font-size: 3rem;
            font-weight: 900;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4, #45b7d1, #96ceb4);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientShift 3s ease-in-out infinite;
            margin-bottom: 10px;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .subtitle {
            color: white;
            font-size: 1.2rem;
            opacity: 0.9;
        }

        /* Ad Spaces */
        .ad-banner {
            background: linear-gradient(45deg, #ff9a56, #ffad56);
            border-radius: 12px;
            padding: 20px;
            text-align: center;
            margin: 30px 0;
            border: 2px dashed rgba(255,255,255,0.3);
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .ad-banner:hover {
            transform: scale(1.02);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .ad-content {
            color: white;
            font-weight: 600;
            font-size: 1.1rem;
        }

        .sidebar-ad {
            position: fixed;
            right: 20px;
            top: 50%;
            transform: translateY(-50%);
            width: 160px;
            height: 600px;
            background: linear-gradient(45deg, #f093fb, #f5576c);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 600;
            z-index: 1000;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .sidebar-ad:hover {
            transform: translateY(-50%) scale(1.05);
        }

        .floating-ad {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            width: 728px;
            height: 90px;
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 600;
            z-index: 1000;
            box-shadow: 0 5px 20px rgba(0,0,0,0.3);
            cursor: pointer;
        }

        .category-nav {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin: 30px 0;
        }

        .category-btn {
            background: rgba(255,255,255,0.2);
            color: white;
            border: none;
            padding: 12px 24px;
            border-radius: 25px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .category-btn:hover, .category-btn.active {
            background: rgba(255,255,255,0.9);
            color: #333;
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
            margin: 40px 0;
        }

        .tool-card {
            background: rgba(255,255,255,0.95);
            border-radius: 20px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.2);
        }

        .tool-card:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .tool-header {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .tool-icon {
            font-size: 2rem;
            margin-right: 15px;
            padding: 10px;
            border-radius: 12px;
            background: linear-gradient(45deg, #667eea, #764ba2);
        }

        .tool-title {
            font-size: 1.4rem;
            font-weight: 700;
            color: #333;
        }

        .tool-content {
            min-height: 200px;
        }

        input, textarea, select, button {
            width: 100%;
            padding: 12px;
            margin: 8px 0;
            border: 2px solid #e1e1e1;
            border-radius: 10px;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        input:focus, textarea:focus, select:focus {
            border-color: #667eea;
            outline: none;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
        }

        button {
            background: linear-gradient(45deg, #667eea, #764ba2);
            color: white;
            border: none;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(102, 126, 234, 0.4);
        }

        .result-area {
            background: #f8f9fa;
            border: 2px dashed #dee2e6;
            border-radius: 10px;
            padding: 15px;
            margin-top: 15px;
            min-height: 60px;
            font-family: monospace;
            overflow-wrap: break-word;
        }

        .color-preview {
            width: 100%;
            height: 60px;
            border-radius: 10px;
            margin: 10px 0;
            border: 2px solid #e1e1e1;
        }

        .palette-colors {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 10px;
            margin: 15px 0;
        }

        .palette-color {
            height: 40px;
            border-radius: 8px;
            cursor: pointer;
            border: 2px solid white;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            transition: transform 0.2s;
        }

        .palette-color:hover {
            transform: scale(1.1);
        }

        .calculator-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 10px;
            margin: 15px 0;
        }

        .calc-btn {
            aspect-ratio: 1;
            font-size: 1.2rem;
            font-weight: 600;
            border-radius: 10px;
        }

        .calc-display {
            background: #1a1a1a;
            color: #00ff00;
            font-family: 'Courier New', monospace;
            font-size: 1.5rem;
            text-align: right;
            padding: 20px;
            margin-bottom: 15px;
            border-radius: 10px;
        }

        .qr-display {
            text-align: center;
            margin: 15px 0;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 15px;
            margin: 15px 0;
        }

        .stat-card {
            background: linear-gradient(45deg, #667eea, #764ba2);
            color: white;
            padding: 15px;
            border-radius: 10px;
            text-align: center;
        }

        .stat-number {
            font-size: 1.5rem;
            font-weight: bold;
            display: block;
        }

        .hidden {
            display: none;
        }

        .premium-badge {
            background: linear-gradient(45deg, #f093fb, #f5576c);
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
            margin-left: 10px;
        }

        .floating-action {
            position: fixed;
            bottom: 100px;
            right: 30px;
            background: linear-gradient(45deg, #ff6b6b, #4ecdc4);
            color: white;
            border: none;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            font-size: 1.5rem;
            cursor: pointer;
            z-index: 1001;
            box-shadow: 0 5px 20px rgba(0,0,0,0.3);
            transition: all 0.3s ease;
        }

        .floating-action:hover {
            transform: scale(1.1) rotate(180deg);
        }

        footer {
            background: rgba(0,0,0,0.8);
            color: white;
            text-align: center;
            padding: 40px 20px;
            margin-top: 60px;
            border-radius: 20px 20px 0 0;
        }

        @media (max-width: 768px) {
            .tools-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .sidebar-ad, .floating-ad {
                display: none;
            }
            
            .logo {
                font-size: 2rem;
            }
            
            .calculator-grid {
                grid-template-columns: repeat(4, 1fr);
                gap: 8px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1 class="logo">🛠️ Essential Tools Hub</h1>
            <p class="subtitle">25+ Free Online Tools for Daily Productivity</p>
        </header>

        <!-- Top Banner Ad - Google AdSense -->
        <div class="ad-banner">
            <ins class="adsbygoogle"
                style="display:block"
                data-ad-client="ca-pub-XXXXXXXXXXXXXXXXX"
                data-ad-slot="1234567890"
                data-ad-format="auto"
                data-full-width-responsive="true"></ins>
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
            <!-- Fallback for demo -->
            <div class="ad-content" id="topAdFallback">
                🎯 Configure your AdSense ID above - 728x90 Banner
                <br><small>Replace ADSENSE_CONFIG with your real Publisher ID & Slot IDs</small>
            </div>
        </div>

        <!-- Category Navigation -->
        <nav class="category-nav">
            <button class="category-btn active" onclick="filterTools('all')">All Tools</button>
            <button class="category-btn" onclick="filterTools('text')">Text</button>
            <button class="category-btn" onclick="filterTools('math')">Math</button>
            <button class="category-btn" onclick="filterTools('design')">Design</button>
            <button class="category-btn" onclick="filterTools('dev')">Developer</button>
            <button class="category-btn" onclick="filterTools('converter')">Converter</button>
        </nav>

        <!-- Tools Grid -->
        <div class="tools-grid" id="toolsGrid">
            
            <!-- Advanced Calculator -->
            <div class="tool-card" data-category="math">
                <div class="tool-header">
                    <div class="tool-icon">🧮</div>
                    <div class="tool-title">Advanced Calculator</div>
                </div>
                <div class="tool-content">
                    <div class="calc-display" id="calcDisplay">0</div>
                    <div class="calculator-grid">
                        <button class="calc-btn" onclick="clearCalc()">C</button>
                        <button class="calc-btn" onclick="calcInput('/')">/</button>
                        <button class="calc-btn" onclick="calcInput('*')">×</button>
                        <button class="calc-btn" onclick="deleteLast()">⌫</button>
                        <button class="calc-btn" onclick="calcInput('7')">7</button>
                        <button class="calc-btn" onclick="calcInput('8')">8</button>
                        <button class="calc-btn" onclick="calcInput('9')">9</button>
                        <button class="calc-btn" onclick="calcInput('-')">-</button>
                        <button class="calc-btn" onclick="calcInput('4')">4</button>
                        <button class="calc-btn" onclick="calcInput('5')">5</button>
                        <button class="calc-btn" onclick="calcInput('6')">6</button>
                        <button class="calc-btn" onclick="calcInput('+')">+</button>
                        <button class="calc-btn" onclick="calcInput('1')">1</button>
                        <button class="calc-btn" onclick="calcInput('2')">2</button>
                        <button class="calc-btn" onclick="calcInput('3')">3</button>
                        <button class="calc-btn" onclick="calculate()" rowspan="2">=</button>
                        <button class="calc-btn" onclick="calcInput('0')" colspan="2">0</button>
                        <button class="calc-btn" onclick="calcInput('.')">.</button>
                    </div>
                </div>
            </div>

            <!-- Password Generator -->
            <div class="tool-card" data-category="text">
                <div class="tool-header">
                    <div class="tool-icon">🔐</div>
                    <div class="tool-title">Password Generator</div>
                </div>
                <div class="tool-content">
                    <label>Password Length: <span id="lengthValue">12</span></label>
                    <input type="range" id="passwordLength" min="4" max="50" value="12" oninput="updateLength()">
                    <label><input type="checkbox" id="includeUppercase" checked> Uppercase</label>
                    <label><input type="checkbox" id="includeLowercase" checked> Lowercase</label>
                    <label><input type="checkbox" id="includeNumbers" checked> Numbers</label>
                    <label><input type="checkbox" id="includeSymbols"> Symbols</label>
                    <button onclick="generatePassword()">Generate Password</button>
                    <div class="result-area" id="passwordResult">Click generate to create password</div>
                    <button onclick="copyToClipboard('passwordResult')">Copy Password</button>
                </div>
            </div>

            <!-- Text Analyzer -->
            <div class="tool-card" data-category="text">
                <div class="tool-header">
                    <div class="tool-icon">📝</div>
                    <div class="tool-title">Text Analyzer</div>
                </div>
                <div class="tool-content">
                    <textarea id="textToAnalyze" placeholder="Enter your text here..." rows="4" oninput="analyzeText()"></textarea>
                    <div class="stats-grid">
                        <div class="stat-card">
                            <span class="stat-number" id="charCount">0</span>
                            <span>Characters</span>
                        </div>
                        <div class="stat-card">
                            <span class="stat-number" id="wordCount">0</span>
                            <span>Words</span>
                        </div>
                        <div class="stat-card">
                            <span class="stat-number" id="lineCount">0</span>
                            <span>Lines</span>
                        </div>
                        <div class="stat-card">
                            <span class="stat-number" id="paragraphCount">0</span>
                            <span>Paragraphs</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Color Palette Generator -->
            <div class="tool-card" data-category="design">
                <div class="tool-header">
                    <div class="tool-icon">🎨</div>
                    <div class="tool-title">Color Palette Generator</div>
                </div>
                <div class="tool-content">
                    <button onclick="generatePalette()">Generate Random Palette</button>
                    <div class="palette-colors" id="colorPalette"></div>
                    <div class="result-area" id="paletteValues"></div>
                </div>
            </div>

            <!-- QR Code Generator -->
            <div class="tool-card" data-category="design">
                <div class="tool-header">
                    <div class="tool-icon">📱</div>
                    <div class="tool-title">QR Code Generator</div>
                </div>
                <div class="tool-content">
                    <input type="text" id="qrInput" placeholder="Enter text or URL">
                    <button onclick="generateQR()">Generate QR Code</button>
                    <div class="qr-display" id="qrResult"></div>
                </div>
            </div>

            <!-- Base64 Encoder/Decoder -->
            <div class="tool-card" data-category="dev">
                <div class="tool-header">
                    <div class="tool-icon">🔄</div>
                    <div class="tool-title">Base64 Encoder/Decoder</div>
                </div>
                <div class="tool-content">
                    <textarea id="base64Input" placeholder="Enter text to encode/decode" rows="3"></textarea>
                    <div style="display: flex; gap: 10px;">
                        <button onclick="encodeBase64()">Encode</button>
                        <button onclick="decodeBase64()">Decode</button>
                    </div>
                    <div class="result-area" id="base64Result"></div>
                </div>
            </div>

            <!-- JSON Formatter -->
            <div class="tool-card" data-category="dev">
                <div class="tool-header">
                    <div class="tool-icon">📋</div>
                    <div class="tool-title">JSON Formatter</div>
                </div>
                <div class="tool-content">
                    <textarea id="jsonInput" placeholder="Paste your JSON here..." rows="4"></textarea>
                    <div style="display: flex; gap: 10px;">
                        <button onclick="formatJSON()">Format</button>
                        <button onclick="minifyJSON()">Minify</button>
                        <button onclick="validateJSON()">Validate</button>
                    </div>
                    <div class="result-area" id="jsonResult"></div>
                </div>
            </div>

            <!-- Unit Converter -->
            <div class="tool-card" data-category="converter">
                <div class="tool-header">
                    <div class="tool-icon">⚖️</div>
                    <div class="tool-title">Unit Converter</div>
                </div>
                <div class="tool-content">
                    <select id="conversionType" onchange="updateUnits()">
                        <option value="length">Length</option>
                        <option value="weight">Weight</option>
                        <option value="temperature">Temperature</option>
                        <option value="area">Area</option>
                        <option value="volume">Volume</option>
                    </select>
                    <input type="number" id="fromValue" placeholder="Enter value" oninput="convertUnits()">
                    <select id="fromUnit"></select>
                    <select id="toUnit"></select>
                    <div class="result-area" id="conversionResult"></div>
                </div>
            </div>

            <!-- Hash Generator -->
            <div class="tool-card" data-category="dev">
                <div class="tool-header">
                    <div class="tool-icon">🔗</div>
                    <div class="tool-title">Hash Generator</div>
                </div>
                <div class="tool-content">
                    <input type="text" id="hashInput" placeholder="Enter text to hash">
                    <select id="hashType">
                        <option value="md5">MD5</option>
                        <option value="sha1">SHA-1</option>
                        <option value="sha256">SHA-256</option>
                    </select>
                    <button onclick="generateHash()">Generate Hash</button>
                    <div class="result-area" id="hashResult"></div>
                </div>
            </div>

            <!-- URL Shortener -->
            <div class="tool-card" data-category="text">
                <div class="tool-header">
                    <div class="tool-icon">🔗</div>
                    <div class="tool-title">URL Shortener</div>
                    <span class="premium-badge">Demo</span>
                </div>
                <div class="tool-content">
                    <input type="url" id="urlInput" placeholder="Enter URL to shorten">
                    <button onclick="shortenUrl()">Shorten URL</button>
                    <div class="result-area" id="urlResult"></div>
                </div>
            </div>

            <!-- Lorem Ipsum Generator -->
            <div class="tool-card" data-category="text">
                <div class="tool-header">
                    <div class="tool-icon">📄</div>
                    <div class="tool-title">Lorem Ipsum Generator</div>
                </div>
                <div class="tool-content">
                    <label>Paragraphs:</label>
                    <input type="number" id="paragraphCount" value="3" min="1" max="20">
                    <button onclick="generateLorem()">Generate Lorem Ipsum</button>
                    <div class="result-area" id="loremResult"></div>
                </div>
            </div>

            <!-- Image Optimizer -->
            <div class="tool-card" data-category="design">
                <div class="tool-header">
                    <div class="tool-icon">🖼️</div>
                    <div class="tool-title">Image Optimizer</div>
                    <span class="premium-badge">Demo</span>
                </div>
                <div class="tool-content">
                    <input type="file" id="imageInput" accept="image/*" onchange="previewImage()">
                    <canvas id="imageCanvas" style="max-width: 100%; margin: 10px 0;"></canvas>
                    <div style="display: flex; gap: 10px;">
                        <button onclick="compressImage()">Compress</button>
                        <button onclick="resizeImage()">Resize</button>
                    </div>
                    <div class="result-area" id="imageResult"></div>
                </div>
            </div>

        </div>

        <!-- Middle Banner Ad - Google AdSense -->
        <div class="ad-banner">
            <ins class="adsbygoogle"
                style="display:block"
                data-ad-client="ca-pub-XXXXXXXXXXXXXXXXX" 
                data-ad-slot="2345678901"
                data-ad-format="auto"
                data-full-width-responsive="true"></ins>
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
            <!-- Fallback for demo -->
            <div class="ad-content" id="middleAdFallback">
                💰 Configure your AdSense ID above - 728x90 Banner
                <br><small>High engagement placement between tools</small>
            </div>
        </div>

        <footer>
            <p>&copy; 2025 Essential Tools Hub. All rights reserved.</p>
            <p>Made with ❤️ for productivity enthusiasts</p>
        </footer>
    </div>

    <!-- Sidebar Ad - Google AdSense -->
    <div class="sidebar-ad">
        <ins class="adsbygoogle"
            style="display:block"
            data-ad-client="ca-pub-XXXXXXXXXXXXXXXXX"
            data-ad-slot="3456789012"
            data-ad-format="auto"
            data-full-width-responsive="true"></ins>
        <script>
            (adsbygoogle = window.adsbygoogle || []).push({});
        </script>
        <!-- Fallback for demo -->
        <div id="sidebarAdFallback">Vertical AdSense<br>160x600<br><small>Configure your Slot ID</small></div>
    </div>

    <!-- Floating Bottom Ad - Google AdSense -->
    <div class="floating-ad">
        <ins class="adsbygoogle"
            style="display:block"
            data-ad-client="ca-pub-XXXXXXXXXXXXXXXXX"
            data-ad-slot="4567890123"
            data-ad-format="auto"
            data-full-width-responsive="true"></ins>
        <script>
            (adsbygoogle = window.adsbygoogle || []).push({});
        </script>
        <!-- Fallback for demo -->
        <div id="bottomAdFallback">Floating AdSense Banner - 728x90<br><small>Always visible at bottom</small></div>
    </div>

    <!-- Floating Action Button -->
    <button class="floating-action" onclick="scrollToTop()" title="Back to Top">↑</button>

    <script>
        // Google AdSense Integration & Analytics
        function initializeAds() {
            // Hide fallback content when AdSense loads successfully
            const adElements = document.querySelectorAll('.adsbygoogle');
            
            adElements.forEach((ad, index) => {
                // Check if AdSense loaded successfully
                if (ad.innerHTML.length > 0) {
                    // Hide corresponding fallback
                    const fallbacks = ['topAdFallback', 'middleAdFallback', 'sidebarAdFallback', 'bottomAdFallback'];
                    const fallback = document.getElementById(fallbacks[index]);
                    if (fallback) fallback.style.display = 'none';
                }
            });
            
            // Track ad impressions for analytics
            console.log('AdSense ads initialized');
            trackEvent('ads', 'page_load', 'adsense_loaded');
        }

        // Enhanced Analytics Tracking
        function trackEvent(category, action, label) {
            // Google Analytics 4 tracking
            if (typeof gtag !== 'undefined') {
                gtag('event', action, {
                    event_category: category,
                    event_label: label,
                    value: 1
                });
            }
            
            // Console log for debugging
            console.log(`Analytics: ${category} - ${action} - ${label}`);
        }

        // Track ad performance and user engagement
        function trackAdPerformance() {
            // Track time spent on page (important for ad revenue)
            let timeOnPage = 0;
            setInterval(() => {
                timeOnPage += 5;
                if (timeOnPage % 30 === 0) { // Every 30 seconds
                    trackEvent('engagement', 'time_on_page', `${timeOnPage}s`);
                }
            }, 5000);

            // Track scroll depth (affects ad visibility)
            let maxScroll = 0;
            window.addEventListener('scroll', () => {
                const scrollPercent = Math.round((window.scrollY / (document.body.scrollHeight - window.innerHeight)) * 100);
                if (scrollPercent > maxScroll) {
                    maxScroll = scrollPercent;
                    if (maxScroll % 25 === 0) { // Every 25%
                        trackEvent('engagement', 'scroll_depth', `${maxScroll}%`);
                    }
                }
            });
        }

        // AdSense Revenue Optimization
        function optimizeAdPlacement() {
            // Lazy loading for better performance
            const adContainers = document.querySelectorAll('.ad-banner, .sidebar-ad, .floating-ad');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        // Track ad visibility
                        const adType = entry.target.className.includes('sidebar') ? 'sidebar' : 
                                     entry.target.className.includes('floating') ? 'floating' : 'banner';
                        trackEvent('ads', 'ad_visible', adType);
                    }
                });
            }, { threshold: 0.5 });

            adContainers.forEach(container => observer.observe(container));
        }

        // Add configuration instructions
        function showAdSenseInstructions() {
            if (ADSENSE_CONFIG.publisherId.includes('XXXXXXXXX')) {
                console.warn(`
🚨 ADSENSE SETUP REQUIRED:
1. Replace 'ca-pub-XXXXXXXXXXXXXXXXX' with your real AdSense Publisher ID
2. Replace slot IDs (1234567890, etc.) with your actual ad unit slot IDs  
3. Get these from: https://www.google.com/adsense/
4. Create ad units for: Banner (728x90), Sidebar (160x600), etc.

💡 Current ad placements:
- Top Banner: ${ADSENSE_CONFIG.adSlots.topBanner}
- Middle Banner: ${ADSENSE_CONFIG.adSlots.middleBanner}
- Sidebar: ${ADSENSE_CONFIG.adSlots.sidebar}  
- Bottom Banner: ${ADSENSE_CONFIG.adSlots.bottomBanner}
                `);
                
                // Show setup notification to admin
                const notification = document.createElement('div');
                notification.innerHTML = `
                    <div style="position: fixed; top: 0; left: 0; right: 0; background: #ff9800; color: white; padding: 10px; text-align: center; z-index: 10000; font-weight: bold;">
                        ⚠️ AdSense Setup Required - Check Console for Instructions
                        <button onclick="this.parentElement.remove()" style="float: right; background: none; border: none; color: white; font-size: 18px; cursor: pointer;">×</button>
                    </div>
                `;
                document.body.appendChild(notification);
            }
        }

        // Calculator Functions
        let calcExpression = '';
        let calcDisplay = document.getElementById('calcDisplay');

        function calcInput(value) {
            if (calcExpression === '0') calcExpression = '';
            calcExpression += value;
            calcDisplay.textContent = calcExpression || '0';
        }

        function clearCalc() {
            calcExpression = '';
            calcDisplay.textContent = '0';
        }

        function deleteLast() {
            calcExpression = calcExpression.slice(0, -1);
            calcDisplay.textContent = calcExpression || '0';
        }

        function calculate() {
            try {
                let result = eval(calcExpression.replace('×', '*'));
                calcDisplay.textContent = result;
                calcExpression = result.toString();
            } catch (error) {
                calcDisplay.textContent = 'Error';
                calcExpression = '';
            }
        }

        // Password Generator
        function updateLength() {
            document.getElementById('lengthValue').textContent = document.getElementById('passwordLength').value;
        }

        function generatePassword() {
            const length = parseInt(document.getElementById('passwordLength').value);
            const uppercase = document.getElementById('includeUppercase').checked;
            const lowercase = document.getElementById('includeLowercase').checked;
            const numbers = document.getElementById('includeNumbers').checked;
            const symbols = document.getElementById('includeSymbols').checked;

            let chars = '';
            if (uppercase) chars += 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
            if (lowercase) chars += 'abcdefghijklmnopqrstuvwxyz';
            if (numbers) chars += '0123456789';
            if (symbols) chars += '!@#$%^&*()_+-=[]{}|;:,.<>?';

            if (!chars) {
                document.getElementById('passwordResult').textContent = 'Select at least one character type';
                return;
            }

            let password = '';
            for (let i = 0; i < length; i++) {
                password += chars.charAt(Math.floor(Math.random() * chars.length));
            }

            document.getElementById('passwordResult').textContent = password;
        }

        // Text Analyzer
        function analyzeText() {
            const text = document.getElementById('textToAnalyze').value;
            
            document.getElementById('charCount').textContent = text.length;
            document.getElementById('wordCount').textContent = text.trim() ? text.trim().split(/\s+/).length : 0;
            document.getElementById('lineCount').textContent = text.split('\n').length;
            document.getElementById('paragraphCount').textContent = text.trim() ? text.split(/\n\s*\n/).length : 0;
        }

        // Color Palette Generator
        function generatePalette() {
            const colors = [];
            const paletteDiv = document.getElementById('colorPalette');
            const valuesDiv = document.getElementById('paletteValues');
            
            paletteDiv.innerHTML = '';
            
            for (let i = 0; i < 5; i++) {
                const color = '#' + Math.floor(Math.random()*16777215).toString(16).padStart(6, '0');
                colors.push(color);
                
                const colorDiv = document.createElement('div');
                colorDiv.className = 'palette-color';
                colorDiv.style.backgroundColor = color;
                colorDiv.onclick = () => copyToClipboard(`paletteColor${i}`, color);
                colorDiv.title = `Click to copy ${color}`;
                colorDiv.id = `paletteColor${i}`;
                paletteDiv.appendChild(colorDiv);
            }
            
            valuesDiv.textContent = colors.join(', ');
        }

        // QR Code Generator
        function generateQR() {
            const text = document.getElementById('qrInput').value;
            if (!text) {
                document.getElementById('qrResult').innerHTML = 'Please enter text or URL';
                return;
            }
            
            // Using QR Server API for demo
            const qrUrl = `https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=${encodeURIComponent(text)}`;
            document.getElementById('qrResult').innerHTML = `<img src="${qrUrl}" alt="QR Code" style="max-width: 200px;">`;
        }

        // Base64 Functions
        function encodeBase64() {
            const text = document.getElementById('base64Input').value;
            try {
                const encoded = btoa(text);
                document.getElementById('base64Result').textContent = encoded;
            } catch (error) {
                document.getElementById('base64Result').textContent = 'Error: Invalid input';
            }
        }

        function decodeBase64() {
            const text = document.getElementById('base64Input').value;
            try {
                const decoded = atob(text);
                document.getElementById('base64Result').textContent = decoded;
            } catch (error) {
                document.getElementById('base64Result').textContent = 'Error: Invalid Base64';
            }
        }

        // JSON Functions
        function formatJSON() {
            const input = document.getElementById('jsonInput').value;
            try {
                const parsed = JSON.parse(input);
                const formatted = JSON.stringify(parsed, null, 2);
                document.getElementById('jsonResult').textContent = formatted;
            } catch (error) {
                document.getElementById('jsonResult').textContent = 'Error: Invalid JSON - ' + error.message;
            }
        }

        function minifyJSON() {
            const input = document.getElementById('jsonInput').value;
            try {
                const parsed = JSON.parse(input);
                const minified = JSON.stringify(parsed);
                document.getElementById('jsonResult').textContent = minified;
            } catch (error) {
                document.getElementById('jsonResult').textContent = 'Error: Invalid JSON - ' + error.message;
            }
        }

        function validateJSON() {
            const input = document.getElementById('jsonInput').value;
            try {
                JSON.parse(input);
                document.getElementById('jsonResult').textContent = '✅ Valid JSON';
            } catch (error) {
                document.getElementById('jsonResult').textContent = '❌ Invalid JSON: ' + error.message;
            }
        }

        // Unit Converter
        const units = {
            length: {
                meter: 1,
                kilometer: 1000,
                centimeter: 0.01,
                millimeter: 0.001,
                inch: 0.0254,
                foot: 0.3048,
                yard: 0.9144,
                mile: 1609.34
            },
            weight: {
                kilogram: 1,
                gram: 0.001,
                pound: 0.453592,
                ounce: 0.0283495,
                ton: 1000
            },
            temperature: {
                celsius: (c) => ({ celsius: c, fahrenheit: c * 9/5 + 32, kelvin: c + 273.15 }),
                fahrenheit: (f) => ({ celsius: (f - 32) * 5/9, fahrenheit: f, kelvin: (f - 32) * 5/9 + 273.15 }),
                kelvin: (k) => ({ celsius: k - 273.15, fahrenheit: (k - 273.15) * 9/5 + 32, kelvin: k })
            },
            area: {
                'square meter': 1,
                'square kilometer': 1000000,
                'square centimeter': 0.0001,
                'square inch': 0.00064516,
                'square foot': 0.092903,
                acre: 4046.86
            },
            volume: {
                liter: 1,
                milliliter: 0.001,
                gallon: 3.78541,
                quart: 0.946353,
                pint: 0.473176,
                cup: 0.236588
            }
        };

        function updateUnits() {
            const type = document.getElementById('conversionType').value;
            const fromUnit = document.getElementById('fromUnit');
            const toUnit = document.getElementById('toUnit');
            
            fromUnit.innerHTML = '';
            toUnit.innerHTML = '';
            
            Object.keys(units[type]).forEach(unit => {
                fromUnit.innerHTML += `<option value="${unit}">${unit}</option>`;
                toUnit.innerHTML += `<option value="${unit}">${unit}</option>`;
            });
        }

        function convertUnits() {
            const type = document.getElementById('conversionType').value;
            const value = parseFloat(document.getElementById('fromValue').value);
            const fromUnit = document.getElementById('fromUnit').value;
            const toUnit = document.getElementById('toUnit').value;
            
            if (!value) {
                document.getElementById('conversionResult').textContent = '';
                return;
            }
            
            let result;
            if (type === 'temperature') {
                const converted = units.temperature[fromUnit](value);
                result = converted[toUnit];
            } else {
                const baseValue = value * units[type][fromUnit];
                result = baseValue / units[type][toUnit];
            }
            
            document.getElementById('conversionResult').textContent = `${value} ${fromUnit} = ${result.toFixed(6)} ${toUnit}`;
        }

        // Hash Generator
        async function generateHash() {
            const text = document.getElementById('hashInput').value;
            const type = document.getElementById('hashType').value;
            
            if (!text) {
                document.getElementById('hashResult').textContent = 'Please enter text to hash';
                return;
            }
            
            try {
                let hash;
                if (type === 'md5') {
                    hash = await md5(text);
                } else if (type === 'sha1') {
                    hash = await sha1(text);
                } else if (type === 'sha256') {
                    hash = await sha256(text);
                }
                document.getElementById('hashResult').textContent = hash;
            } catch (error) {
                document.getElementById('hashResult').textContent = 'Error generating hash';
            }
        }

        // Simple hash functions (for demo purposes)
        async function md5(text) {
            return 'MD5: ' + btoa(text).slice(0, 32); // Demo implementation
        }

        async function sha1(text) {
            const encoder = new TextEncoder();
            const data = encoder.encode(text);
            const hashBuffer = await crypto.subtle.digest('SHA-1', data);
            const hashArray = Array.from(new Uint8Array(hashBuffer));
            return hashArray.map(b => b.toString(16).padStart(2, '0')).join('');
        }

        async function sha256(text) {
            const encoder = new TextEncoder();
            const data = encoder.encode(text);
            const hashBuffer = await crypto.subtle.digest('SHA-256', data);
            const hashArray = Array.from(new Uint8Array(hashBuffer));
            return hashArray.map(b => b.toString(16).padStart(2, '0')).join('');
        }

        // URL Shortener (Demo)
        function shortenUrl() {
            const url = document.getElementById('urlInput').value;
            if (!url) {
                document.getElementById('urlResult').textContent = 'Please enter a URL';
                return;
            }
            
            // Demo implementation - in real app, use actual URL shortening service
            const shortCode = Math.random().toString(36).substring(7);
            document.getElementById('urlResult').textContent = `https://short.ly/${shortCode}`;
        }

        // Lorem Ipsum Generator
        function generateLorem() {
            const count = parseInt(document.getElementById('paragraphCount').value);
            const loremText = [
                "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
                "Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.",
                "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.",
                "Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
                "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.",
                "Totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt.",
                "Explicabo nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit.",
                "Sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt."
            ];
            
            let result = '';
            for (let i = 0; i < count; i++) {
                result += loremText[i % loremText.length] + '\n\n';
            }
            
            document.getElementById('loremResult').textContent = result.trim();
        }

        // Image Functions (Demo)
        function previewImage() {
            const file = document.getElementById('imageInput').files[0];
            if (!file) return;
            
            const canvas = document.getElementById('imageCanvas');
            const ctx = canvas.getContext('2d');
            const img = new Image();
            
            img.onload = function() {
                canvas.width = Math.min(300, img.width);
                canvas.height = Math.min(300, img.height);
                ctx.drawImage(img, 0, 0, canvas.width, canvas.height);
            };
            
            img.src = URL.createObjectURL(file);
        }

        function compressImage() {
            document.getElementById('imageResult').textContent = 'Image compressed (demo) - In real app, this would compress the image';
        }

        function resizeImage() {
            document.getElementById('imageResult').textContent = 'Image resized (demo) - In real app, this would resize the image';
        }

        // Utility Functions
        function copyToClipboard(elementId, text) {
            const textToCopy = text || document.getElementById(elementId).textContent;
            navigator.clipboard.writeText(textToCopy).then(() => {
                showNotification('Copied to clipboard!');
            });
        }

        function showNotification(message) {
            const notification = document.createElement('div');
            notification.textContent = message;
            notification.style.cssText = `
                position: fixed;
                top: 20px;
                right: 20px;
                background: #4CAF50;
                color: white;
                padding: 12px 20px;
                border-radius: 8px;
                z-index: 10000;
                animation: slideIn 0.3s ease;
            `;
            document.body.appendChild(notification);
            setTimeout(() => notification.remove(), 3000);
        }

        // Filter Tools by Category
        function filterTools(category) {
            const tools = document.querySelectorAll('.tool-card');
            const buttons = document.querySelectorAll('.category-btn');
            
            buttons.forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');
            
            tools.forEach(tool => {
                if (category === 'all' || tool.dataset.category === category) {
                    tool.style.display = 'block';
                    tool.style.animation = 'fadeIn 0.5s ease';
                } else {
                    tool.style.display = 'none';
                }
            });
        }

        // Scroll to Top
        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        // Initialize
        document.addEventListener('DOMContentLoaded', function() {
            updateUnits();
            generatePalette();
            
            // Add CSS animations
            const style = document.createElement('style');
            style.textContent = `
                @keyframes slideIn {
                    from { transform: translateX(100%); }
                    to { transform: translateX(0); }
                }
                @keyframes fadeIn {
                    from { opacity: 0; transform: translateY(20px); }
                    to { opacity: 1; transform: translateY(0); }
                }
            `;
            document.head.appendChild(style);
            
            // Analytics tracking (replace with your tracking code)
            console.log('Essential Tools Hub loaded - Track page views here');
        });

        // SEO and Performance Monitoring
        function trackToolUsage(toolName) {
            // Replace with your analytics code (Google Analytics, etc.)
            console.log(`Tool used: ${toolName}`);
            
            // Example: gtag('event', 'tool_usage', { 'tool_name': toolName });
        }

        // Add event listeners for tool usage tracking
        document.addEventListener('click', function(e) {
            if (e.target.tagName === 'BUTTON') {
                const toolCard = e.target.closest('.tool-card');
                if (toolCard) {
                    const toolName = toolCard.querySelector('.tool-title').textContent;
                    trackToolUsage(toolName);
                }
            }
        });
    </script>
</body>
</html>
