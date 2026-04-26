<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SIM Computer - Abakassé</title>
    <style>
        /* CSS : Le Design */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f7f6;
            color: #333;
        }

        header {
            background-color: #004a99;
            color: white;
            padding: 20px;
            text-align: center;
        }

        .container {
            width: 90%;
            max-width: 1000px;
            margin: 20px auto;
        }

        .info-contact {
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            margin-bottom: 20px;
            text-align: center;
        }

        .grille-produits {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .carte {
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }

        .carte:hover {
            transform: scale(1.05);
        }

        .carte img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 5px;
        }

        .prix {
            font-size: 1.2em;
            color: #d9534f;
            font-weight: bold;
        }

        .btn-whatsapp {
            display: inline-block;
            background-color: #25D366;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 10px;
            font-weight: bold;
        }

        .services {
            background: #e9ecef;
            padding: 20px;
            margin-top: 30px;
            border-radius: 8px;
        }

        footer {
            text-align: center;
            padding: 20px;
            font-size: 0.9em;
            color: #666;
        }
    </style>
</head>
<body>

<header>
    <h1>SIM Computer</h1>
    <p>Votre partenaire informatique à Abakassé</p>
</header>

<div class="container">
    
    <div class="info-contact">
        <h2>📍 Localisation : Marché A, Abakassé</h2>
        <p>📱 WhatsApp : <strong>650701289</strong></p>
        <a href="https://wa.me/237650701289" class="btn-whatsapp">Commander par WhatsApp</a>
    </div>

    <h2 style="text-align:center;">Nos Articles</h2>
    
    <div class="grille-produits">
        <div class="carte">
            <img src="https://images.unsplash.com/photo-1588872657578-7efd1f1555ed?w=400" alt="Ordinateur entrée de gamme">
            <h3>Ordinateur Bureautique</h3>
            <p>Idéal pour secrétariat et études.</p>
            <p class="prix">70 000 FCFA</p>
            <button onclick="commander('Ordinateur 70k')" class="btn-whatsapp">Réserver</button>
        </div>

        <div class="carte">
            <img src="https://images.unsplash.com/photo-1525547719571-a2d4ac8945e2?w=400" alt="Laptop puissant">
            <h3>Laptop Professionnel</h3>
            <p>Haute performance, Core i5/i7.</p>
            <p class="prix">250 000 FCFA</p>
            <button onclick="commander('Laptop 250k')" class="btn-whatsapp">Réserver</button>
        </div>

        <div class="carte">
            <img src="https://images.unsplash.com/photo-1527864550417-7fd91fc51a46?w=400" alt="Accessoires">
            <h3>Accessoires</h3>
            <p>Souris, Claviers, Disques durs.</p>
            <p class="prix">Dès 5 000 FCFA</p>
            <button onclick="commander('Accessoires')" class="btn-whatsapp">Voir plus</button>
        </div>
    </div>

    <div class="services">
        <h3>🛠 Nos Services</h3>
        <ul>
            <li>Vente de Laptops et Desktops</li>
            <li>Réparation de machines</li>
            <li>Installation de logiciels (Office, Antivirus, Systèmes)</li>
        </ul>
    </div>

</div>

<footer>
    &copy; 2024 SIM Computer - Tous droits réservés.
</footer>

<script>
    /* JavaScript : L'interaction */
    function commander(produit) {
        const message = "Bonjour SIM Computer, je suis intéressé par : " + produit;
        const numero = "237650701289";
        const url = "https://wa.me/" + numero + "?text=" + encodeURIComponent(message);
        window.open(url, '_blank');
    }
</script>

</body>
</html>
