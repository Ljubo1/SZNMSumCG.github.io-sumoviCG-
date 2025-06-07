# SZNMSumCG.github.io-sumoviCG-
<!DOCTYPE html>
<html lang="sr">
<head>
  <meta charset="UTF-8">
  <title>Služba za nadzor mreže i servisa</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      text-align: center;
      padding: 40px;
    }

    h1 {
      font-size: 28px;
      margin-bottom: 40px;
    }

    select, button {
      padding: 10px 15px;
      font-size: 16px;
      margin: 10px;
    }
  </style>
</head>
<body>
  <h1>Služba za nadzor mreže i servisa</h1>

  <div>
    <select id="dugmad">
      <option value="">-- Izaberi dugme --</option>
      <!-- Automatski punimo dugmad putem JS -->
    </select>
    <button onclick="otvori()">Otvori</button>
  </div>

  <script>
    const select = document.getElementById('dugmad');

    // Napravi 25 opcija
    for (let i = 1; i <= 25; i++) {
      const option = document.createElement('option');
      option.value = i;
      option.textContent = `Dugme ${i}`;
      select.appendChild(option);
    }

    function otvori() {
      const broj = select.value;
      if (!broj) return;

      const html = `
        <!DOCTYPE html>
        <html lang="sr">
        <head>
          <meta charset="UTF-8">
          <title>Dugme ${broj}</title>
        </head>
        <body>
          <h2>Dugme ${broj} – Unos teksta</h2>
          <textarea rows="15" cols="80" placeholder="Ovde unesite tekst..."></textarea>
        </body>
        </html>
      `;

      const encoded = encodeURIComponent(html)
        .replace(/'/g, '%27')
        .replace(/"/g, '%22');

      const dataUrl = 'data:text/html;charset=utf-8,' + encoded;

      window.open(dataUrl, '_blank');
    }
  </script>
</body>
</html>
