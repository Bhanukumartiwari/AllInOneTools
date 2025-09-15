<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Free online tools for text, passwords, conversions, coding, and more – essential utilities for developers, students, and professionals">
    <meta name="keywords" content="online tools, password generator, unit converter, QR code generator, JSON formatter, base64 encoder">
    <title>Essential Tools Hub - Multi-Purpose Web Tools</title>
    <!-- Manifest for PWA -->
    <link rel="manifest" href="data:application/manifest+json;base64,eyJuYW1lIjoiRXNzZW50aWFsIFRvb2xzIEh1YiIsInNob3J0X25hbWUiOiJUb29sc0h1YiIsInN0YXJ0X3VybCI6Ii8iLCJkaXNwbGF5Ijoic3RhbmRhbG9uZSIsImJhY2tncm91bmRfY29sb3IiOiIjZmZmZmZmIiwidGhlbWVfY29sb3IiOiIjMDA3YWZmIiwiaWNvbnMiOlt7InNyYyI6Imh0dHBzOi8vZXhhbXBsZS5jb20vaWNvbi5wbmciLCJzaXplcyI6IjE5MngxOTIiLCJ0eXBlIjoiaW1hZ2UvcG5nIn1dfQ==">
    <style>
        /* Embedded CSS */
        :root {
            --primary-color: #007aff;
            --secondary-color: #34c759;
            --accent-color: #ff9500;
            --bg-color: #f4f4f4;
            --text-color: #333;
            --dark-bg: #1c1c1e;
            --dark-text: #fff;
        }
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: var(--bg-color);
            color: var(--text-color);
            transition: background 0.3s, color 0.3s;
        }
        body.dark-mode {
            background: var(--dark-bg);
            color: var(--dark-text);
        }
        header {
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 1rem;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 10;
        }
        nav {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1rem;
            margin: 1rem 0;
        }
        nav a {
            text-decoration: none;
            color: var(--text-color);
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: background 0.3s;
        }
        nav a:hover {
            background: rgba(0,122,255,0.1);
        }
        .tool-section {
            margin: 2rem auto;
            max-width: 1200px;
            padding: 1rem;
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            animation: fadeIn 0.5s;
        }
        body.dark-mode .tool-section {
            background: #2c2c2e;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        input, button, select, textarea {
            padding: 0.5rem;
            margin: 0.5rem 0;
            border: 1px solid #ddd;
            border-radius: 5px;
            transition: border 0.3s;
        }
        input:focus, textarea:focus {
            border-color: var(--primary-color);
            outline: none;
        }
        button {
            background: var(--primary-color);
            color: white;
            cursor: pointer;
            transition: background 0.3s;
        }
        button:hover {
            background: #0056b3;
        }
        .output {
            margin-top: 1rem;
            padding: 1rem;
            background: #f8f9fa;
            border-radius: 5px;
            word-break: break-all;
        }
        body.dark-mode .output {
            background: #3a3a3c;
        }
        .ad-space {
            background: #eee;
            padding: 1rem;
            text-align: center;
            margin: 1rem 0;
            border-radius: 5px;
        }
        body.dark-mode .ad-space {
            background: #3a3a3c;
        }
        #search-bar {
            width: 100%;
            max-width: 600px;
            margin: 1rem auto;
            display: block;
        }
        .premium-btn {
            background: var(--accent-color);
            color: white;
        }
        .copy-btn {
            margin-left: 0.5rem;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background: var(--primary-color);
            color: white;
        }
        /* More styles for specific tools */
        .color-preview {
            width: 50px;
            height: 50px;
            border: 1px solid #ddd;
            display: inline-block;
        }
        canvas {
            border: 1px solid #ddd;
        }
        pre {
            background: #f4f4f4;
            padding: 1rem;
            overflow: auto;
        }
        body.dark-mode pre {
            background: #1c1c1e;
        }
        /* Grid layout */
        .tools-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1rem;
        }
        @media (max-width: 600px) {
            .tools-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Essential Tools Hub</h1>
        <p>Multi-Purpose Web Tools for Developers, Students, and Professionals</p>
        <!-- Ad Banner Here -->
        <div class="ad-space" id="header-ad">Header Ad Banner</div>
        <input type="text" id="search-bar" placeholder="Search tools..." oninput="searchTools()">
        <button onclick="toggleDarkMode()">Toggle Dark Mode</button>
    </header>
    <nav>
        <a href="#text-tools">Text Tools</a>
        <a href="#security-tools">Security</a>
        <a href="#converters">Converters</a>
        <a href="#coding-utils">Coding Utils</a>
        <a href="#other-tools">Other Tools</a>
        <a href="#blog">Blog</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>
    <main class="tools-grid">
        <section id="text-tools" class="tool-section">
            <h2>Text Utilities</h2>
            <p>For developers and writers: Convert case, count words, reverse text.</p>
            <textarea id="text-input" placeholder="Enter text"></textarea>
            <button onclick="convertCase('upper')">Uppercase</button>
            <button onclick="convertCase('lower')">Lowercase</button>
            <button onclick="convertCase('title')">Title Case</button>
            <button onclick="countWords()">Count Words/Chars</button>
            <button onclick="reverseText()">Reverse Text</button>
            <div class="output" id="text-output"></div>
            <button class="copy-btn" onclick="copyToClipboard('text-output')">Copy</button>
            <button class="premium-btn" onclick="showPremiumModal('Text Tools')">Upgrade to Premium</button>
            <!-- Ad Here -->
            <div class="ad-space">Sidebar Ad</div>
        </section>

        <section id="password-generator" class="tool-section">
            <h2>Password Generator</h2>
            <p>Secure passwords for everyone.</p>
            <label>Length: <input type="number" id="pw-length" value="12" min="4"></label>
            <label>Include Numbers: <input type="checkbox" id="pw-numbers" checked></label>
            <label>Include Symbols: <input type="checkbox" id="pw-symbols" checked></label>
            <label>Include Uppercase: <input type="checkbox" id="pw-upper" checked></label>
            <button onclick="generatePassword()">Generate</button>
            <div class="output" id="pw-output"></div>
            <meter id="pw-strength" value="0" max="1"></meter>
            <button class="copy-btn" onclick="copyToClipboard('pw-output')">Copy</button>
        </section>

        <section id="unit-converter" class="tool-section">
            <h2>Unit Converter</h2>
            <p>Convert units for students and professionals.</p>
            <input type="number" id="unit-input" placeholder="Value">
            <select id="unit-from">
                <option value="m">Meters</option>
                <option value="ft">Feet</option>
                <!-- Add more -->
            </select>
            <select id="unit-to">
                <option value="ft">Feet</option>
                <option value="m">Meters</option>
            </select>
            <button onclick="convertUnit()">Convert</button>
            <div class="output" id="unit-output"></div>
            <!-- Currency placeholder -->
            <p>Basic currency (hardcoded rates)</p>
        </section>

        <section id="color-utils" class="tool-section">
            <h2>Color Utilities</h2>
            <p>For designers and marketers.</p>
            <input type="color" id="color-picker" onchange="updateColor()">
            <div class="color-preview" id="color-preview"></div>
            <button onclick="generatePalette()">Generate Palette</button>
            <div id="palette-output" class="output"></div>
            <select id="color-format">
                <option>HEX</option>
                <option>RGB</option>
                <option>HSL</option>
            </select>
            <div class="output" id="color-output"></div>
        </section>

        <section id="qr-generator" class="tool-section">
            <h2>QR Code Generator</h2>
            <input id="qr-input" placeholder="Text or URL">
            <button onclick="generateQR()">Generate</button>
            <canvas id="qr-canvas" width="200" height="200"></canvas>
            <a id="qr-download" download="qr.png">Download</a>
        </section>

        <section id="calculator" class="tool-section">
            <h2>Smart Calculator</h2>
            <input id="calc-input" placeholder="Expression">
            <button onclick="calculate()">Calculate</button>
            <div class="output" id="calc-output"></div>
            <div id="calc-history"></div>
        </section>

        <section id="json-formatter" class="tool-section">
            <h2>JSON Formatter/Validator</h2>
            <p>For developers.</p>
            <textarea id="json-input" placeholder="Paste JSON"></textarea>
            <button onclick="formatJSON()">Format</button>
            <button onclick="validateJSON()">Validate</button>
            <pre id="json-output"></pre>
        </section>

        <section id="base64" class="tool-section">
            <h2>Base64 Encoder/Decoder</h2>
            <textarea id="base64-input" placeholder="Text"></textarea>
            <button onclick="encodeBase64()">Encode</button>
            <button onclick="decodeBase64()">Decode</button>
            <div class="output" id="base64-output"></div>
        </section>

        <section id="url-shortener" class="tool-section">
            <h2>URL Shortener</h2>
            <input id="url-input" placeholder="Long URL">
            <button onclick="shortenURL()">Shorten</button>
            <div class="output" id="short-url"></div>
        </section>

        <section id="image-resizer" class="tool-section">
            <h2>Image Resizer/Compressor</h2>
            <input type="file" id="image-file" accept="image/*">
            <label>Width: <input type="number" id="resize-width"></label>
            <label>Height: <input type="number" id="resize-height"></label>
            <button onclick="resizeImage()">Resize</button>
            <canvas id="image-canvas"></canvas>
            <a id="image-download" download="resized.jpg">Download</a>
        </section>

        <section id="hash-generator" class="tool-section">
            <h2>Hash Generator</h2>
            <textarea id="hash-input" placeholder="Text"></textarea>
            <select id="hash-type">
                <option>MD5</option>
                <option>SHA1</option>
                <option>SHA256</option>
            </select>
            <button onclick="generateHash()">Generate</button>
            <div class="output" id="hash-output"></div>
        </section>

        <section id="md-to-html" class="tool-section">
            <h2>Markdown to HTML Converter</h2>
            <textarea id="md-input" placeholder="Markdown"></textarea>
            <button onclick="convertMD()">Convert</button>
            <div id="html-output" class="output"></div>
        </section>

        <section id="lorem-ipsum" class="tool-section">
            <h2>Lorem Ipsum Generator</h2>
            <label>Paragraphs: <input type="number" id="lorem-paras" value="3"></label>
            <button onclick="generateLorem()">Generate</button>
            <div class="output" id="lorem-output"></div>
        </section>

        <section id="timezone-converter" class="tool-section">
            <h2>Timezone Converter</h2>
            <input type="datetime-local" id="tz-input">
            <select id="tz-from">
                <option>UTC</option>
                <!-- Add more -->
            </select>
            <select id="tz-to">
                <option>PST</option>
            </select>
            <button onclick="convertTimezone()">Convert</button>
            <div class="output" id="tz-output"></div>
        </section>

        <section id="ip-lookup" class="tool-section">
            <h2>IP Address Lookup</h2>
            <button onclick="lookupIP()">Lookup My IP</button>
            <div class="output" id="ip-output">IP: Demo 192.168.0.1, Country: USA</div>
        </section>

        <section id="site-speed" class="tool-section">
            <h2>Website Speed Test</h2>
            <input id="speed-url" placeholder="URL">
            <button onclick="testSpeed()">Test</button>
            <div class="output" id="speed-output"></div>
        </section>

        <section id="css-minifier" class="tool-section">
            <h2>CSS Minifier</h2>
            <textarea id="css-input" placeholder="CSS"></textarea>
            <button onclick="minifyCSS()">Minify</button>
            <div class="output" id="css-output"></div>
        </section>

        <section id="code-beautifier" class="tool-section">
            <h2>HTML/CSS/JS Beautifier</h2>
            <textarea id="code-input" placeholder="Code"></textarea>
            <select id="code-type">
                <option>HTML</option>
                <option>CSS</option>
                <option>JS</option>
            </select>
            <button onclick="beautifyCode()">Beautify</button>
            <pre id="code-output"></pre>
        </section>

    </main>

    <section id="blog" class="tool-section">
        <h2>Blog</h2>
        <article>
            <h3>How to Use Our Password Generator Securely</h3>
            <p>Content here...</p>
        </article>
        <!-- More articles -->
    </section>

    <section id="about" class="tool-section">
        <h2>About</h2>
        <p>Essential Tools Hub is a collection of free online tools.</p>
    </section>

    <section id="contact" class="tool-section">
        <h2>Contact</h2>
        <form>
            <input placeholder="Name">
            <input placeholder="Email">
            <textarea placeholder="Message"></textarea>
            <button type="submit">Send</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Essential Tools Hub</p>
        <a href="https://github.com/yourrepo">GitHub Repo</a>
        <p>Privacy Policy | Terms</p>
        <!-- Email Signup -->
        <form action="#" method="post">
            <input type="email" placeholder="Subscribe to Newsletter">
            <button type="submit">Subscribe</button>
        </form>
        <!-- Ad Footer -->
        <div class="ad-space">Footer Ad</div>
    </footer>

    <!-- Premium Modal -->
    <div id="premium-modal" style="display:none; position:fixed; top:50%; left:50%; transform:translate(-50%,-50%); background:white; padding:2rem; border-radius:10px; box-shadow:0 0 10px rgba(0,0,0,0.5);">
        <h3>Upgrade to Premium</h3>
        <p>Unlock advanced features!</p>
        <a href="https://affiliate-link.com">Learn More</a>
        <button onclick="closeModal()">Close</button>
    </div>

    <script>
        // Embedded JavaScript
        // Utility functions
        function copyToClipboard(id) {
            const el = document.getElementById(id);
            navigator.clipboard.writeText(el.innerText).then(() => alert('Copied!'));
        }

        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
        }

        function searchTools() {
            const query = document.getElementById('search-bar').value.toLowerCase();
            const sections = document.querySelectorAll('.tool-section');
            sections.forEach(sec => {
                sec.style.display = sec.textContent.toLowerCase().includes(query) ? 'block' : 'none';
            });
        }

        function showPremiumModal(tool) {
            document.getElementById('premium-modal').style.display = 'block';
        }

        function closeModal() {
            document.getElementById('premium-modal').style.display = 'none';
        }

        // Text Utilities
        function convertCase(type) {
            const input = document.getElementById('text-input').value;
            let output = '';
            if (type === 'upper') output = input.toUpperCase();
            else if (type === 'lower') output = input.toLowerCase();
            else if (type === 'title') output = input.replace(/\b\w/g, c => c.toUpperCase());
            document.getElementById('text-output').innerText = output;
        }

        function countWords() {
            const input = document.getElementById('text-input').value;
            const words = input.trim().split(/\s+/).length;
            const chars = input.length;
            document.getElementById('text-output').innerText = `Words: ${words}, Characters: ${chars}`;
        }

        function reverseText() {
            const input = document.getElementById('text-input').value;
            document.getElementById('text-output').innerText = input.split('').reverse().join('');
        }

        // Password Generator
        function generatePassword() {
            const length = parseInt(document.getElementById('pw-length').value);
            const numbers = document.getElementById('pw-numbers').checked;
            const symbols = document.getElementById('pw-symbols').checked;
            const upper = document.getElementById('pw-upper').checked;
            let chars = 'abcdefghijklmnopqrstuvwxyz';
            if (upper) chars += 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
            if (numbers) chars += '0123456789';
            if (symbols) chars += '!@#$%^&*()';
            let pw = '';
            for (let i = 0; i < length; i++) {
                pw += chars.charAt(Math.floor(Math.random() * chars.length));
            }
            document.getElementById('pw-output').innerText = pw;
            const strength = (length > 8 && numbers && symbols && upper) ? 0.9 : 0.5;
            document.getElementById('pw-strength').value = strength;
        }

        // Unit Converter (simple example for length)
        function convertUnit() {
            const value = parseFloat(document.getElementById('unit-input').value);
            const from = document.getElementById('unit-from').value;
            const to = document.getElementById('unit-to').value;
            let result;
            if (from === 'm' && to === 'ft') result = value * 3.28084;
            else if (from === 'ft' && to === 'm') result = value / 3.28084;
            // Add more conversions
            document.getElementById('unit-output').innerText = result;
        }

        // Color Utilities
        function updateColor() {
            const color = document.getElementById('color-picker').value;
            document.getElementById('color-preview').style.background = color;
            const format = document.getElementById('color-format').value;
            let out = color;
   # AllInOneTools
