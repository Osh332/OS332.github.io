# OS332.github<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KS Wielcy</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Verdana, sans-serif;
            background-color: #f0f8ff;
            color: #000;
            line-height: 1.6;
        }
        header {
            background-color: #267326;
            padding: 20px;
            text-align: center;
            color: #fff;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            animation: slideInDown 1s ease-in-out;
        }
        nav {
            background-color: #ffd700;
            padding: 10px;
            text-align: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        nav ul li {
            margin: 5px 20px;
        }
        nav ul li a {
            color: #000;
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            transition: color 0.3s, background-color 0.3s;
        }
        nav ul li a:hover {
            color: #fff;
            background-color: #267326;
            border-radius: 5px;
        }
        main {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
            animation: fadeIn 1.5s ease-in-out;
        }
        section {
            margin-bottom: 50px;
        }
        h1 {
            color: #fff;
            font-size: 2.5em;
            animation: zoomIn 1s ease-in-out;
        }
        h2 {
            color: #008080;
            font-size: 2em;
            border-bottom: 2px solid #267326;
            display: inline-block;
            margin-bottom: 20px;
        }
        p {
            margin-bottom: 20px;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 10px;
        }
        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 5px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        footer {
            background-color: #267326;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
            }
            nav ul li {
                margin: 10px 0;
            }
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes slideInDown {
            from {
                opacity: 0;
                transform: translateY(-100%);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes zoomIn {
            from {
                opacity: 0;
                transform: scale(0.5);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        .contact-form {
            display: flex;
            flex-direction: column;
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
        }
        .contact-form input,
        .contact-form textarea {
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1em;
            transition: border-color 0.3s;
        }
        .contact-form input:focus,
        .contact-form textarea:focus {
            border-color: #267326;
        }
        .contact-form button {
            padding: 10px;
            border: none;
            border-radius: 5px;
            background-color: #267326;
            color: #fff;
            font-size: 1.2em;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }
        .contact-form button:hover {
            background-color: #195319;
            transform: scale(1.05);
        }
        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            max-width: 100%;
            background: #000;
            margin-bottom: 50px;
        }
        .video-container iframe,
        .video-container object,
        .video-container embed {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        .btn {
            display: inline-block;
            padding: 10px 20px;
            font-size: 1em;
            color: #fff;
            background-color: #267326;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.3s;
        }
        .btn:hover {
            background-color: #195319;
            transform: scale(1.05);
        }
        .carousel {
            display: flex;
            overflow-x: auto;
            scroll-behavior: smooth;
        }
        .carousel img {
            min-width: 100%;
            transition: transform 0.5s ease;
        }
        .carousel img:hover {
            transform: scale(1.1);
        }
    </style>
</head>
<body>
    <header>
        <h1>Witaj na stronie klubu KS Wielcy</h1>
    </header>
    
    <nav>
        <ul>
            <li><a href="#informacje">Informacje</a></li>
            <li><a href="#zdjecia">Zdjęcia</a></li>
            <li><a href="#terminarz">Terminarz</a></li>
            <li><a href="#kontakt">Kontakt</a></li>
        </ul>
    </nav>
    
    <main>
        <section id="informacje">
            <h2>Informacje</h2>
            <p>Tutaj znajdziesz najważniejsze informacje o klubie KS Wielcy.</p>
            <p>Klub Sportowy Wielcy to zespół z pasją i determinacją do osiągania sukcesów. Nasze barwy to żółty, niebieski, zielony i biały, symbolizujące naszą energię, siłę, świeżość i ducha sportowego.</p>
        </section>
        
        <section id="zdjecia">
            <h2>Zdjęcia</h2>
            <p>Tutaj znajdziesz galerię zdjęć z meczów i wydarzeń klubowych.</p>
            <div class="carousel">
                <img src="https://via.placeholder.com/1200x600" alt="Zdjęcie 1">
                <img src="https://via.placeholder.com/1200x600" alt="Zdjęcie 2">
                <img src="https://via.placeholder.com/1200x600" alt="Zdjęcie 3">
            </div>
        </section>
        
        <section id="terminarz">
            <h2>Terminarz</h2>
            <p>Sprawdź nadchodzące mecze i wydarzenia:</p>
            <ul>
                <li>01.06.2024 - KS Wielcy vs. Drużyna A</li>
                <li>08.06.2024 - KS Wielcy vs. Drużyna B</li>
                <li>15.06.2024 - KS Wielcy vs. Drużyna C</li>
                <li>22.06.2024 - KS Wielcy vs. Drużyna D</li>
            </ul>
        </section>
        
        <section id="kontakt">
            <h2>Kontakt</h2>
            <p>Skontaktuj się z nami, używając poniższego formularza:</p>
            <div class="contact-form">
                <input type="text" placeholder="Twoje
.io
