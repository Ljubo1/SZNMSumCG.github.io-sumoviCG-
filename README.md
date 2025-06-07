# SZNMSumCG.github.io-sumoviCG-
<ŠUMOVI U CG>
<!DOCTYPE html>
<html lang="sr">
<head>
    <meta charset="UTF-8">
    <title>Služba za nadzor mreže i servisa</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
        }
        h1 {
            color: #333;
        }
        select {
            padding: 10px;
            font-size: 16px;
        }
    </style>
    <script>
        function otvoriGrad(stranica) {
            if (stranica !== "") {
                window.location.href = `gradovi/${stranica}.html`;
            }
        }
    </script>
</head>
<body>
    <h1>Služba za nadzor mreže i servisa</h1>

    <label for="gradovi">Izaberite grad:</label>
    <select id="gradovi" onchange="otvoriGrad(this.value)">
        <option value="">-- Izaberi grad --</option>
        <option value="PG_Mtel">PG_Mtel</option>
        <option value="PG_Stari_Aerodrom">PG_Stari Aerodrom</option>
        <option value="PG_Bazar">PG_Bazar</option>
        <option value="PG_City_Quart">PG_City Quart</option>
        <option value="PG_AutoZeta">PG_AutoZeta</option>
        <option value="PG_Zelenika">PG_Zelenika</option>
        <option value="Cetinje">Cetinje</option>
        <option value="Tivat">Tivat</option>
        <option value="Herceg_Novi">Herceg Novi</option>
        <option value="Igalo">Igalo</option>
        <option value="Budva">Budva</option>
        <option value="Bečići">Bečići</option>
        <option value="Petrovac">Petrovac</option>
        <option value="Bar">Bar</option>
        <option value="Ulcinj">Ulcinj</option>
        <option value="Nikšić">Nikšić</option>
        <option value="Pljevlja">Pljevlja</option>
        <option value="Bijelo_Polje">Bijelo Polje</option>
        <option value="Berane">Berane</option>
        <option value="Rožaje">Rožaje</option>
        <option value="Mojkovac">Mojkovac</option>
        <option value="Andrijevica">Andrijevica</option>
    </select>
</body>
</html>
