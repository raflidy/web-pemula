<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Cek Kecocokan Zodiak</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(to right, #fbc2eb, #a6c1ee);
      padding: 50px;
      text-align: center;
    }
    h1 {
      color: #333;
    }
    select, button {
      padding: 10px;
      margin: 10px;
      font-size: 16px;
    }
    #hasil {
      margin-top: 20px;
      font-weight: bold;
      font-size: 18px;
      color: #222;
    }
  </style>
</head>
<body>

  <h1>🌟 Cek Kecocokan Zodiak 🌟</h1>

  <label for="zodiak1">Zodiak Kamu:</label><br>
  <select id="zodiak1">
    <option>Aries</option>
    <option>Taurus</option>
    <option>Gemini</option>
    <option>Cancer</option>
    <option>Leo</option>
    <option>Virgo</option>
    <option>Libra</option>
    <option>Scorpio</option>
    <option>Sagittarius</option>
    <option>Capricorn</option>
    <option>Aquarius</option>
    <option>Pisces</option>
  </select><br>

  <label for="zodiak2">Zodiak Pasangan:</label><br>
  <select id="zodiak2">
    <option>Aries</option>
    <option>Taurus</option>
    <option>Gemini</option>
    <option>Cancer</option>
    <option>Leo</option>
    <option>Virgo</option>
    <option>Libra</option>
    <option>Scorpio</option>
    <option>Sagittarius</option>
    <option>Capricorn</option>
    <option>Aquarius</option>
    <option>Pisces</option>
  </select><br>

  <button onclick="cekKecocokan()">Cek Kecocokan</button>

  <div id="hasil"></div>

  <script>
    function cekKecocokan() {
      const zodiak1 = document.getElementById("zodiak1").value;
      const zodiak2 = document.getElementById("zodiak2").value;
      let hasil = "";

      if (zodiak1 === zodiak2) {
        hasil = "💖 Kalian sangat cocok, pasangan zodiak yang sejiwa!";
      } else if (
        (zodiak1 === "Leo" && zodiak2 === "Aries") ||
        (zodiak1 === "Aries" && zodiak2 === "Leo") ||
        (zodiak1 === "Cancer" && zodiak2 === "Pisces") ||
        (zodiak1 === "Pisces" && zodiak2 === "Cancer") ||
        (zodiak1 === "Taurus" && zodiak2 === "Virgo") ||
        (zodiak1 === "Virgo" && zodiak2 === "Taurus")
        (zodiak1 === "Capricorn" && zodiak2 === "Gemini")
      ) {
        hasil = "😍 Kalian pasangan yang sangat serasi!";
      } else {
        hasil = "🙂 Kecocokan kalian sedang-sedang saja, tapi cinta bisa tumbuh kok!";
      } else {
        hasil = "🤭 Kalian sangat cocok harus sampai menikah!";

      document.getElementById("hasil").innerText = hasil;
    }
  </script>

</body>
</html>
