<h1>FreshMart - Premium Organic E-Commerce Store 🌿</h1>

<p>A modern, responsive, and fully functional front-end implementation for <strong>FreshMart</strong>, a Sri Lankan SME specializing in organic food products. This project was developed as part of the <em>Enterprise Cloud and Infrastructure Automation</em> module.</p>

<h2>📖 Overview</h2>
<p>This repository contains the source code for the FreshMart client-side application. It is a single-page application (SPA) designed to be hosted on <strong>Amazon S3</strong> as a static website. It features a clean, professional user interface with interactive elements like a shopping cart, product filtering, and mobile responsiveness.</p>

<h2>✨ Key Features</h2>
<ul>
    <li><strong>Responsive Design:</strong> Fully fluid layout that adapts to Desktop, Tablet, and Mobile screens.</li>
    <li><strong>Modern UI/UX:</strong> Built with a "Glassmorphism" navigation bar, smooth scroll animations, and a clean color palette.</li>
    <li><strong>Interactive Shopping Cart:</strong>
        <ul>
            <li>Add items to the cart without reloading the page.</li>
            <li>Real-time subtotal calculation.</li>
            <li>Slide-out cart drawer UI.</li>
            <li>Remove items dynamically.</li>
        </ul>
    </li>
    <li><strong>Product Filtering:</strong> JavaScript-based filtering system to toggle between categories (Vegetables, Fruits, Dairy).</li>
    <li><strong>Toast Notifications:</strong> Non-intrusive popup notifications when actions are performed (e.g., "Item added to cart").</li>
    <li><strong>Zero Dependencies:</strong> Uses <strong>Tailwind CSS via CDN</strong>, meaning no <code>npm install</code> or build step is required to run this project.</li>
</ul>

<h2>🛠 Technologies Used</h2>
<ul>
    <li><strong>HTML5:</strong> Semantic markup.</li>
    <li><strong>Tailwind CSS (CDN):</strong> Utility-first CSS framework for rapid UI development.</li>
    <li><strong>JavaScript (ES6+):</strong> Vanilla JS for DOM manipulation, cart logic, and state management.</li>
    <li><strong>Font Awesome:</strong> For iconography.</li>
</ul>

<h2>🚀 How to Run Locally</h2>
<ol>
    <li>
        <strong>Clone the repository:</strong>
        <pre><code>git clone https://github.com/Sanda1113/freshmart-website.git</code></pre>
    </li>
    <li>
        <strong>Navigate to the folder:</strong>
        <pre><code>cd freshmart-website</code></pre>
    </li>
    <li>
        <strong>Open the file:</strong><br>
        Simply double-click <code>index.html</code> to open it in your default web browser.<br>
        <em>Alternatively, if using VS Code, use the "Live Server" extension.</em>
    </li>
</ol>

<h2>☁️ Deployment (AWS S3)</h2>
<p>This project is optimized for AWS S3 Static Website Hosting.</p>
<ol>
    <li>Create an <strong>S3 Bucket</strong> in the AWS Console.</li>
    <li>Upload <code>index.html</code> to the root of the bucket.</li>
    <li>Enable <strong>Static Website Hosting</strong> in the bucket properties.</li>
    <li>Add a <strong>Bucket Policy</strong> to allow public read access:
<pre><code>{
"Version": "2012-10-17",
"Statement": [
    {
        "Sid": "PublicReadGetObject",
        "Effect": "Allow",
        "Principal": "*",
        "Action": "s3:GetObject",
        "Resource": "arn:aws:s3:::YOUR-BUCKET-NAME/*"
    }
]
}</code></pre>
    </li>
    <li>Access the site via the provided S3 Endpoint URL.</li>
</ol>

<h2>📂 Project Structure</h2>
<pre><code>/
├── index.html      # Main entry point containing HTML, CSS (Tailwind), and JS
└── README.html     # Project documentation</code></pre>

<h2>👤 Author</h2>
<ul>
    <li><strong>Student ID:</strong> CB014568</li>
    <li><strong>Module:</strong> COMP50008 - Enterprise Cloud and Infrastructure Automation 1</li>
</ul>

<hr>
<p><em>This project is for educational purposes only.</em></p>
