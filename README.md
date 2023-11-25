
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Message d'amour quotidien</title>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            text-align: center;
            margin: 50px;
            background-color: #ffe8e8;
            transition: background-color 1s ease;
        }

        #loading {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #fff;
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 999;
        }

        #love-message {
            font-size: 24px;
            margin-top: 50px;
            opacity: 0;
            transition: opacity 1s ease;
            display: inline-block;
            color: #8e44ad;
        }

        #love-message.show {
            opacity: 1;
        }

        @keyframes appear {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        span {
            display: inline-block;
            opacity: 0;
            animation: appear 0.5s ease-in-out forwards;
        }

        span:nth-child(1) { animation-delay: 0.1s; }
        span:nth-child(2) { animation-delay: 0.2s; }
        span:nth-child(3) { animation-delay: 0.3s; }
        span:nth-child(4) { animation-delay: 0.4s; }
        span:nth-child(5) { animation-delay: 0.5s; }
        span:nth-child(6) { animation-delay: 0.6s; }
        span:nth-child(7) { animation-delay: 0.7s; }
        span:nth-child(8) { animation-delay: 0.8s; }
        span:nth-child(9) { animation-delay: 0.9s; }
        span:nth-child(10) { animation-delay: 1s; }
        span:nth-child(11) { animation-delay: 1.1s; }
        span:nth-child(12) { animation-delay: 1.2s; }
        e règles que nécessaire pour chaque mot */

    </style>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap">
</head>
<body>

<div id="loading">Chargement...</div>

<h1>Bonjour Hulda Karen Danielle,</h1>
<p>Voici votre message d'amour du jour :</p>

<div id="love-message" class="show">
    <span>Tu</span>
    <span>es</span>
    <span>la</span>
    <span>lumière</span>
    <span>de</span>
    <span>ma</span>
    <span>vie.</span>
    <span>Ma</span>
    <span>journée</span>
    <span>commence</span>
    <span>et</span>
    <span>se</span>
    <span>termine</span>
    <span>avec</span>
    <span>toi</span>
    <span>dans</span>
    <span>mes</span>
    <span>pensées.</span>
</div>

<script>
    if ('serviceWorker' in navigator) {
        navigator.serviceWorker.register('service-worker.js')
            .then(registration => {
                console.log('Service Worker enregistré avec succès:', registration);
            })
            .catch(error => {
                console.error('Erreur d\'enregistrement du Service Worker:', error);
            });
    }

    const loveMessages = [
    "Hulda Karen Danielle, tu es la lumière de ma vie.",
    "Ma journée commence et se termine avec toi, Hulda Karen Danielle, dans mes pensées.",
    "Ton sourire, Hulda Karen Danielle, rend chaque jour plus beau.",
    "Mon amour pour toi, Hulda Karen Danielle, est aussi profond que l'océan.",
    "À tes côtés, Hulda Karen Danielle, chaque moment est une éternité.",
    "Chaque regard échangé avec toi, Hulda Karen Danielle, est une promesse d'amour.",
    "Ta présence, Hulda Karen Danielle, remplit mon cœur de bonheur.",
    "Mon amour pour toi, Hulda Karen Danielle, grandit de jour en jour.",
    "Tu es la raison, Hulda Karen Danielle, pour laquelle je crois en l'amour éternel.",
    "Chaque jour avec toi, Hulda Karen Danielle, est une aventure extraordinaire.",
    "Ton amour, Hulda Karen Danielle, est le plus précieux des cadeaux.",
    "À travers toutes les saisons, Hulda Karen Danielle, mon amour pour toi persiste.",
    "Tu es mon âme sœur, Hulda Karen Danielle, ma moitié parfaite.",
    "Avec toi, Hulda Karen Danielle, chaque jour est une bénédiction.",
    "Ton amour, Hulda Karen Danielle, est la musique de mon cœur.",
    "Chaque moment passé avec toi, Hulda Karen Danielle, est gravé dans mon âme.",
    "Tu es la personne, Hulda Karen Danielle, que j'ai toujours cherchée.",
    "Mon amour pour toi, Hulda Karen Danielle, est une flamme qui ne s'éteint jamais.",
    "Ta voix, Hulda Karen Danielle, est ma mélodie préférée.",
    "À chaque battement de mon cœur, Hulda Karen Danielle, je pense à toi.",
    "Tu es la plus belle étoile dans mon ciel, Hulda Karen Danielle.",
    // ... 480 autres messages uniques
    "Avec toi, Hulda Karen Danielle, chaque jour est une nouvelle aventure.",
    "Ton amour illumine même les jours les plus sombres, Hulda Karen Danielle.",
    "Chaque sourire que tu m'offres, Hulda Karen Danielle, est une caresse pour mon cœur.",
    "Tu es la clé, Hulda Karen Danielle, qui ouvre les portes de mon bonheur.",
    "Mon amour pour toi, Hulda Karen Danielle, est une histoire sans fin.",
    "À travers les hauts et les bas, Hulda Karen Danielle, notre amour persiste.",
    "Chaque jour avec toi, Hulda Karen Danielle, est un cadeau précieux.",
    "Tu es le rêve devenu réalité, Hulda Karen Danielle, que je ne cesse de vivre.",
    "Mon amour pour toi, Hulda Karen Danielle, est plus fort que tous les obstacles.",
    "À chaque lever de soleil, Hulda Karen Danielle, je me réjouis de t'aimer.",
    "Tu es mon refuge, Hulda Karen Danielle, mon amour éternel.",
    "Chaque moment partagé avec toi, Hulda Karen Danielle, est une perle rare.",
    "Mon amour pour toi, Hulda Karen Danielle, est la force qui guide mes pas.",
    "Ton amour, Hulda Karen Danielle, est mon havre de paix.",
    "Les étoiles pâlissent devant la beauté de ton sourire, Hulda Karen Danielle.",
    "Mon cœur bat au rythme de ton amour, Hulda Karen Danielle.",
    "À travers les vents du temps, notre amour reste immuable, Hulda Karen Danielle.",
    "Chaque mot doux que tu dis, Hulda Karen Danielle, réchauffe mon cœur.",
    "Ta gentillesse, Hulda Karen Danielle, est un trésor que je chéris chaque jour.",
    "Tu es la muse qui inspire les poèmes de mon âme, Hulda Karen Danielle.",
    "La douceur de tes étreintes, Hulda Karen Danielle, est mon refuge.",
        // ... Ajoutez autant de messages que vous le souhaitez
    ];

    function getDayOfYear() {
        const now = new Date();
        const start = new Date(now.getFullYear(), 0, 0);
        const diff = now - start;
        const oneDay = 1000 * 60 * 60 * 24;
        const dayOfYear = Math.floor(diff / oneDay);
        return dayOfYear;
    }

    function hideLoading() {
        const loadingElement = document.getElementById('loading');
        loadingElement.style.display = 'none';
    }

    const dayOfYear = getDayOfYear();
    const loveMessageIndex = dayOfYear % loveMessages.length;
    const loveMessage = loveMessages[loveMessageIndex];

    const loveMessageElement = document.getElementById('love-message');
    loveMessageElement.innerHTML = loveMessage.split(' ').map(word => `<span>${word}</span>`).join(' ');

    setTimeout(() => {
        loveMessageElement.classList.add('show');
        hideLoading();
    }, 500);
</script>

</body>
</html>
