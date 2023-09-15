<!DOCTYPE html>
<html lang="no">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kattens Verden</title>
    <style>
        /* Felles stiler for nettsiden din */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        /* Standardstiler for nettsideelementene */
        header {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px;
        }

        /* Resten av CSS-stilene dine */

        /* Hover-animasjon for hver seksjon */
        section {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background-color: #fff;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
            margin-bottom: 20px;
            transition: transform 0.2s; /* Legg til en overgang for transformasjonsegenskapen */
        }

        section:hover {
            transform: scale(1.05); /* Øk størrelsen ved hover */
        }
    </style>
</head>
<body>
    <header>
        <h1>Velkommen til Kattens Verden</h1>
        <nav>
            <ul>
                <li><a href="#home" class="nav-link">Hjem</a></li>
                <li><a href="#about" class="nav-link">Om Oss</a></li>
                <li><a href="#cats" class="nav-link">Våre Katter</a></li>
                <li><a href="#contact" class="nav-link">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h2>Hjem</h2>
        <p>Velkommen til Kattens Verden - det ultimate nettstedet for katteelskere over hele verden. Her kan du dykke dypt inn i den fascinerende kattens verden.</p>
    </section>

    <section id="about">
        <h2>Om Oss</h2>
        <p>Vi er et fellesskap av katteentusiaster som er lidenskapelige opptatt av alt som har med katter å gjøre. Vår misjon er å informere, underholde og inspirere katteelskere i alle aldre. </p>
    </section>

    <section id="cats">
        <h2>Våre Katter</h2>
        <p>Møt våre katter:</p>
        <ul>
<h1>Charlie - Søtest</h1>
            <li><img src="cat1.jpg" alt="Katt 1" title="Charlie - Søtest"></li>
            <h1>Maya - Kulest</h1>
            <li><img src="cat2.jpg" alt="Katt 2" title="Maya - Kulest"></li>
          <h1>Tiga - Styggest</h1>
            <li><img src="cat3.jpg.jpg" alt="Katt 3" title="Ginger - Syggest"></li>
        </ul>
    </section>

    <!-- Legg til flere seksjoner og innhold her for å gjøre koden lenger -->

    <section id="fun-facts">
        <h2>Morsomme Kattfakta</h2>
        <ul>
            <li>Katter har vært tamme i over 4 000 år.</li>
            <li>Verdens eldste katt ble 38 år gammel.</li>
            <li>Katter kan lage over 100 forskjellige lyder.</li>
            <li>Den gjennomsnittlige katten sover 12-16 timer om dagen.</li>
        </ul>
    </section>
    <section id="testimonials">
        <h2>Hva Våre Besøkende Sier</h2>
        <div class="testimonial">
            <p>"Jeg elsker dette nettstedet! Det er et paradis for katteelskere!"</p>
            <cite>— Stein Henrik Vestly</cite>
        </div>
        <div class="testimonial">
            <p>"Jeg besøker Kattens Verden hver dag for min daglige dose av søthet!"</p>
            <cite>— Lukas Poecevicius</cite>
        </div>
    </section>

    <!-- Mer innhold og seksjoner kan legges til etter behov -->

    <section id="contact">
        <h2>Kontakt Oss</h2>
        <p>Hvis du vil ta kontakt:</p>
        <address>
            E-post: <a href="mailto:ericsinfo@kattensverden.no">ericsinfo@kattensverden.no</a><br>
            Telefon: 939-48-369<br>
            Adresse: 123 Kattegate, Mjauville
        </address>
    </section>

    <footer>
        <p>&copy; 2023 Kattens Verden. Alle rettigheter reservert.</p>
    </footer>

    <script>
        // Jevn rulling ved klikk på navigasjonslenker
        document.querySelectorAll('.nav-link').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();

                const targetId = this.getAttribute('href').substring(1);
                const targetElement = document.getElementById(targetId);

                window.scrollTo({
                    top: targetElement.offsetTop,
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
