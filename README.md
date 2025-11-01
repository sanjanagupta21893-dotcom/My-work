# My-work
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>HTML Formatting Demo</title>
  <style>
    /* Page background and default font */
    body {
      background: linear-gradient(135deg, #f0f8ff 0%, #fffaf0 100%);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: #222;
      padding: 28px;
      line-height: 1.6;
    }

    /* Headings with different fonts / weights */
    h1 { font-family: Georgia, 'Times New Roman', serif; font-weight: 700; }
    h2 { font-family: 'Courier New', Courier, monospace; font-weight: 600; }

    /* Colored text examples */
    .red { color: #d32f2f; }
    .blue { color: #1565c0; }
    .green { color: #2e7d32; }

    /* Underline example (more control than <u>) */
    .fancy-underline { text-decoration: underline; text-decoration-color: #ff8a65; text-decoration-thickness: 2px; }

    /* Blinking text using CSS animation (replacement for deprecated <blink>) */
    @keyframes blink { 0%,50% { opacity: 1 } 50.01%,100% { opacity: 0 } }
    .blink {
      animation: blink 1s steps(1, end) infinite;
      font-weight: 700;
    }

    /* A subtle card for demo blocks */
    .card {
      background: rgba(255,255,255,0.9);
      border-radius: 10px;
      padding: 16px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.08);
      margin-bottom: 18px;
    }

    /* Small helper for font-size & width example */
    .wide { max-width: 900px; }
    .narrow { max-width: 360px; }

    /* Example of colored horizontal rule */
    hr.fancy { border: 0; height: 4px; background: linear-gradient(90deg,#ff8a65,#ffd54f); border-radius: 4px; }
  </style>
</head>
<body>
  <div class="card wide">
    <h1>HTML Formatting Demo</h1>
    <p><strong>Bold</strong> — use the <code>&lt;strong&gt;</code> or <code>&lt;b&gt;</code> tag for bold text.</p>
    <p><em>Italics</em> — use the <code>&lt;em&gt;</code> or <code>&lt;i&gt;</code> tag for emphasis/italic text.</p>
    <p><u>Underline</u> — the <code>&lt;u&gt;</code> tag adds an underline. You can also use CSS (see the orange underline below):</p>
    <p class="fancy-underline">This text uses a colored, thicker underline via CSS.</p>

    <h2 class="blue">Colors, Font &amp; Font Weight</h2>
    <p class="red"><strong>Red text</strong> (class <code>.red</code>), <span class="green">green text</span> (class <code>.green</code>), and <span style="font-family: 'Palatino Linotype', 'Book Antiqua', Palatino, serif; font-weight: 800; font-size: 1.1rem;">a serif example with heavier weight</span>.</p>

    <h2 class="blue">Paragraphs, Line Breaks &amp; Horizontal Line</h2>
    <p>This is one paragraph. To create a new paragraph use the <code>&lt;p&gt;</code> tag which automatically adds spacing.</p>
    <p>This is another paragraph. Insert a manual line break using <code>&lt;br&gt;</code>:<br>Line after a break.</p>

    <hr class="fancy">

    <h2>Marquee and Blinking Text</h2>
    <p>Marquee text (deprecated but still supported in some browsers):</p>
    <marquee behavior="scroll" direction="left" scrollamount="6">This is a <strong>marquee</strong> — scrolling text using &lt;marquee&gt; (deprecated).</marquee>

    <p style="margin-top:12px;">Blinking text using CSS animation (recommended instead of &lt;blink&gt;): <span class="blink">This text blinks.</span></p>

    <h2>Font Width (max-width example) &amp; Background</h2>
    <div class="card narrow">
      <p>This box demonstrates a narrower column (simulating "width") — change <code>max-width</code> or use CSS <code>width</code> to control element width. The page background uses a gradient applied on the <code>&lt;body&gt;</code>.</p>
    </div>

    <h2>Miscellaneous Examples</h2>
    <p>You can mix formatting: <strong><em><u class="fancy-underline">bold, italic and underlined</u></em></strong> text with a <span style="color:#6a1b9a;">custom color</span>.</p>

    <p>Links, lists and images work the same — here's a short unordered list:</p>
    <ul>
      <li><strong>Bold item</strong></li>
      <li><em>Italic item</em></li>
      <li><u>Underlined item</u></li>
    </ul>

    <p>End of demo. Save this file as <code>formatted_example.html</code> and open it in your browser to see everything.</p>
  </div>
</body>
</html>
