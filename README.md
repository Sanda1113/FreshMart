FreshMart - Premium Organic E-Commerce Store 🌿

A modern, responsive, and fully functional front-end implementation for FreshMart, a Sri Lankan SME specializing in organic food products. This project was developed as part of the Enterprise Cloud and Infrastructure Automation module.

📖 Overview

This repository contains the source code for the FreshMart client-side application. It is a single-page application (SPA) designed to be hosted on Amazon S3 as a static website. It features a clean, professional user interface with interactive elements like a shopping cart, product filtering, and mobile responsiveness.

✨ Key Features

Responsive Design: Fully fluid layout that adapts to Desktop, Tablet, and Mobile screens.

Modern UI/UX: Built with a "Glassmorphism" navigation bar, smooth scroll animations, and a clean color palette.

Interactive Shopping Cart:

Add items to the cart without reloading the page.

Real-time subtotal calculation.

Slide-out cart drawer UI.

Remove items dynamically.

Product Filtering: JavaScript-based filtering system to toggle between categories (Vegetables, Fruits, Dairy).

Toast Notifications: Non-intrusive popup notifications when actions are performed (e.g., "Item added to cart").

Zero Dependencies: Uses Tailwind CSS via CDN, meaning no npm install or build step is required to run this project.

🛠 Technologies Used

HTML5: Semantic markup.

Tailwind CSS (CDN): Utility-first CSS framework for rapid UI development.

JavaScript (ES6+): Vanilla JS for DOM manipulation, cart logic, and state management.

Font Awesome: For iconography.

🚀 How to Run Locally

Clone the repository:

git clone [https://github.com/your-username/freshmart-website.git](https://github.com/your-username/freshmart-website.git)


Navigate to the folder:

cd freshmart-website


Open the file:
Simply double-click index.html to open it in your default web browser.
Alternatively, if using VS Code, use the "Live Server" extension.

☁️ Deployment (AWS S3)

This project is optimized for AWS S3 Static Website Hosting.

Create an S3 Bucket in the AWS Console.

Upload index.html to the root of the bucket.

Enable Static Website Hosting in the bucket properties.

Add a Bucket Policy to allow public read access:

{
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
}


Access the site via the provided S3 Endpoint URL.

📂 Project Structure

/
├── index.html      # Main entry point containing HTML, CSS (Tailwind), and JS
└── README.md       # Project documentation


👤 Author

Student ID: [Your ID Here]

Module: COMP50008 - Enterprise Cloud and Infrastructure Automation 1

This project is for educational purposes only.
