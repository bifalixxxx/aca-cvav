<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Trousseau Colo</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f4f4f8;
      margin: 0;
      padding: 0;
    }

    header {
      text-align: center;
      padding: 20px;
      background-color: #ffffff;
      border-bottom: 2px solid #ddd;
    }

    header img {
      height: 80px;
    }

    h1 {
      margin-top: 10px;
      font-size: 1.8em;
      color: #333;
    }

    .intro {
      text-align: center;
      padding: 40px 20px;
    }

    .alert-box {
      background-color: #fff4e5;
      border: 1px solid #ffcc80;
      color: #8a6d3b;
      padding: 20px;
      margin: 20px auto;
      max-width: 600px;
      border-radius: 8px;
      font-size: 1em;
      display: none;
    }

    .start-btn {
      background-color: #333;
      color: white;
      padding: 12px 24px;
      font-size: 1em;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      margin-top: 20px;
    }

    main {
      max-width: 900px;
      margin: auto;
      padding: 30px 20px;
      display: none;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      background-color: #fff;
      box-shadow: 0 0 10px rgba(0,0,0,0.05);
    }

    th, td {
      padding: 12px;
      border-bottom: 1px solid #e0e0e0;
      text-align: left;
    }

    th {
      background-color: #fafafa;
    }

    input[type="checkbox"] {
      transform: scale(1.2);
    }

    input[type="number"] {
      width: 60px;
      padding: 5px;
    }

    @media (max-width: 600px) {
      td, th {
        font-size: 0.9em;
      }

      h1 {
        font-size: 1.4em;
      }
    }
  </style>
</head>
<body>

<header>
  <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%2Fid%2FOIP.AnmCQ-n-zxtelDi_T-StFwHaFP%3Fpid%3DApi&f=1&ipt=2309d25d149a6680948a82a9ad09756b149f637c295773ca661897ea005e098b&ipo=images" alt="Logo">
  <h1>Trousseau à glisser à l'intérieur de la valise</h1>
</header>

<div class="intro">
  <button id="startBtn" class="start-btn" onclick="showChecklist()">Commencer</button>
</div>

<div class="alert-box" id="alertBox">
  <strong>MERCI DE MARQUER LE LINGE AU NOM DE L'ENFANT.</strong><br><br>
  Chaque année, nous rencontrons des difficultés avec le linge mal marqué.<br>
  Nous déclinons toute responsabilité pour les vêtements égarés, parce que non identifiés.
</div>

<main id="checklist">
  <table>
    <thead>
      <tr>
        <th>Équipement</th>
        <th>Présent ?</th>
        <th>Quantité</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>1 paire de draps ou sac de couchage</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>2 pyjamas</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>2 serviettes de toilette et gants</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>1 maillot de bain + bonnet piscine</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>1 serviette de bain</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>5 paquets de Kleenex</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>4 tee-shirts</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>6 culottes/slips/caleçons</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>6 paires de chaussettes</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>2 pulls ou gilets</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>1 K-Way ou équipement pluie</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>1 paire de pantoufles</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>2 paires de chaussures</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>1 paire abîmée (rafting)</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>2 pantalons</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>4 shorts</td><td><input type="checkbox"></td><td><input type="number" min="0"></td></tr>
      <tr><td>Nécessaire de toilette</td><td><input type="checkbox"></td><td></td></tr>
      <tr><td>1 peignoir</td><td><input type="checkbox"></td><td></td></tr>
      <tr><td>1 gourde (nouvelle)</td><td><input type="checkbox"></td><td></td></tr>
      <tr><td>1 sac à dos (nouveau)</td><td><input type="checkbox"></td><td></td></tr>
      <tr><td>1 stick pour les lèvres</td><td><input type="checkbox"></td><td></td></tr>
      <tr><td>1 crème solaire adaptée</td><td><input type="checkbox"></td><td></td></tr>
      <tr><td>1 stylo, lettres, adresses</td><td><input type="checkbox"></td><td></td></tr>
    </tbody>
  </table>
</main>

<script>
  function showChecklist() {
    document.getElementById('startBtn').style.display = 'none';
    document.getElementById('alertBox').style.display = 'block';
    setTimeout(() => {
      const checklist = document.getElementById('checklist');
      checklist.style.display = 'block';
      // Correction iPhone : scroll classique
      window.scrollTo({ top: checklist.offsetTop, behavior: 'auto' });
    }, 2500);
  }
</script>

</body>
</html>
