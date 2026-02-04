jj<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JOSHUA-RICH AGRO-TECH INDUSTRIES LIMITED</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-green: #2d5a27;
            --secondary-green: #4a7c59;
            --accent-green: #6b9e82;
            --light-green: #e8f5e9;
            --brown: #8b5a2b;
            --light-brown: #f5f0e6;
            --white: #ffffff;
            --gray: #666666;
            --light-gray: #f8f9fa;
            --dark-gray: #333333;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark-gray);
            background-color: var(--white);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header & Navigation */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo img {
            height: 50px;
            width: auto;
        }

        .logo-text {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-green);
        }

        .nav-links {
            display: flex;
            gap: 25px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark-gray);
            font-weight: 600;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--primary-green);
        }

        .cta-button {
            background-color: var(--primary-green);
            color: var(--white);
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s ease;
        }

        .cta-button:hover {
            background-color: var(--secondary-green);
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--primary-green);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(45, 90, 39, 0.85), rgba(45, 90, 39, 0.9)), url('https://placehold.co/1200x600/2d5a27/ffffff?text=Nigerian+Farms') no-repeat center center/cover;
            color: var(--white);
            padding: 100px 0;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            justify-content: center;
        }

        .btn-primary {
            background-color: var(--white);
            color: var(--primary-green);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.1rem;
            transition: transform 0.3s ease;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .btn-secondary {
            background-color: transparent;
            color: var(--white);
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.1rem;
            border: 2px solid var(--white);
            transition: background-color 0.3s ease;
        }

        .btn-secondary:hover {
            background-color: var(--white);
            color: var(--primary-green);
        }

        /* Section Styling */
        section {
            padding: 80px 0;
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-header h2 {
            font-size: 2.5rem;
            color: var(--primary-green);
            margin-bottom: 15px;
        }

        .section-header p {
            color: var(--gray);
            max-width: 700px;
            margin: 0 auto;
        }

        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .about-text h3 {
            font-size: 2rem;
            color: var(--primary-green);
            margin-bottom: 20px;
        }

        .about-text p {
            margin-bottom: 15px;
        }

        .about-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        .mission-vision {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .card {
            background: var(--white);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            text-align: center;
        }

        .card i {
            font-size: 3rem;
            color: var(--primary-green);
            margin-bottom: 20px;
        }

        .card h4 {
            font-size: 1.5rem;
            color: var(--primary-green);
            margin-bottom: 15px;
        }

        /* Products & Services */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: var(--white);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
        }

        .service-image {
            height: 200px;
            background-color: var(--light-green);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-green);
            font-size: 3rem;
        }

        .service-content {
            padding: 25px;
        }

        .service-content h4 {
            font-size: 1.3rem;
            color: var(--primary-green);
            margin-bottom: 10px;
        }

        /* Solutions */
        .solutions-tabs {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 40px;
        }

        .tab-btn {
            padding: 10px 25px;
            background: var(--light-green);
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .tab-btn.active, .tab-btn:hover {
            background: var(--primary-green);
            color: var(--white);
        }

        .solution-content {
            background: var(--light-green);
            padding: 40px;
            border-radius: 15px;
            text-align: center;
        }

        /* Blog */
        .blog-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .blog-card {
            background: var(--white);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }

        .blog-image {
            height: 200px;
            background-color: var(--light-brown);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--brown);
            font-size: 3rem;
        }

        .blog-content {
            padding: 25px;
        }

        .blog-content h4 {
            font-size: 1.3rem;
            color: var(--primary-green);
            margin-bottom: 10px;
        }

        .blog-meta {
            color: var(--gray);
            font-size: 0.9rem;
            margin-bottom: 15px;
        }

        /* Contact */
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 25px;
        }

        .contact-item {
            display: flex;
            gap: 15px;
            align-items: flex-start;
        }

        .contact-item i {
            color: var(--primary-green);
            font-size: 1.2rem;
            margin-top: 5px;
        }

        .contact-form {
            background: var(--white);
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: var(--dark-gray);
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }

        .form-group textarea {
            height: 120px;
            resize: vertical;
        }

        /* Footer */
        footer {
            background: var(--primary-green);
            color: var(--white);
            padding: 60px 0 30px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-column h4 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-column h4::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background: var(--accent-green);
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 10px;
        }

        .footer-links a {
            color: var(--light-green);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: var(--white);
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            color: var(--white);
            text-decoration: none;
            transition: background 0.3s ease;
        }

        .social-links a:hover {
            background: var(--accent-green);
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 0.9rem;
            color: var(--light-green);
        }

        /* Edit Button */
        .edit-btn {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: var(--primary-green);
            color: white;
            padding: 12px 24px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            z-index: 1001;
            transition: all 0.3s ease;
        }

        .edit-btn:hover {
            background: var(--secondary-green);
            transform: translateY(-2px);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 15px;
            }

            .nav-links {
                flex-wrap: wrap;
                justify-content: center;
            }

            .hero h1 {
                font-size: 2.2rem;
            }

            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .section-header h2 {
                font-size: 2rem;
            }
        }

        @media (max-width: 480px) {
            .mobile-menu-btn {
                display: block;
            }

            .nav-links {
                display: none;
            }

            .hero {
                padding: 60px 0;
            }

            .hero h1 {
                font-size: 1.8rem;
            }

            .btn-primary, .btn-secondary {
                padding: 10px 20px;
                font-size: 1rem;
            }
    «jj<!DOCTYPE html>
