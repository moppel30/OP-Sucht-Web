<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<title>OPSUCHT Market – Alle Items</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background: linear-gradient(135deg, #2d2d2d 0%, #1a1a1a 100%);
        color: #e0e0e0;
        padding: 25px;
        min-height: 100vh;
    }

    h1 {
        color: #ff9800;
        text-align: center;
        font-size: 2.5em;
        text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        margin-bottom: 30px;
    }

    h2 {
        margin-top: 40px;
        color: #ff9800;
        border-bottom: 3px solid #ff9800;
        padding-bottom: 8px;
        font-size: 1.8em;
    }

    button {
        padding: 15px 30px;
        font-size: 18px;
        cursor: pointer;
        background: linear-gradient(135deg, #ff9800 0%, #f57c00 100%);
        border: none;
        border-radius: 8px;
        margin-bottom: 25px;
        color: white;
        font-weight: bold;
        box-shadow: 0 4px 15px rgba(255, 152, 0, 0.4);
        transition: all 0.3s ease;
    }

    button:hover {
        background: linear-gradient(135deg, #fb8c00 0%, #e65100 100%);
        transform: translateY(-2px);
        box-shadow: 0 6px 20px rgba(255, 152, 0, 0.5);
    }

    table {
        width: 100%;
        border-collapse: collapse;
        margin-top: 15px;
        background: #3a3a3a;
        border-radius: 10px;
        overflow: hidden;
        box-shadow: 0 4px 15px rgba(0,0,0,0.3);
    }

    th, td {
        border: 1px solid #555;
        padding: 12px;
        text-align: center;
    }

    th {
        background: #2a2a2a;
        color: #ff9800;
        font-weight: bold;
        font-size: 16px;
    }

    tr:nth-child(even) {
        background: #333;
    }

    tr:nth-child(odd) {
        background: #3a3a3a;
    }

    tr:hover {
        background: #404040;
    }

    .buy {
        color: #4caf50;
        font-weight: bold;
        font-size: 15px;
    }

    .sell {
        color: #f44336;
        font-weight: bold;
        font-size: 15px;
    }

    .status {
        margin-top: 15px;
        font-style: italic;
        text-align: center;
        font-size: 18px;
        color: #ff9800;
        padding: 15px;
        background: rgba(255, 152, 0, 0.1);
        border-radius: 8px;
        border: 2px solid #ff9800;
    }
</style>
</head>
<body>

<h1>🎮 OPSUCHT Marktpreise</h1>

<button onclick="loadMarket()">📊 Alle Items laden</button>

<div id="status" class="status"></div>
<div id="content"></div>

<script>
async function loadMarket() {
    const status = document.getElementById("status");
    const content = document.getElementById("content");

    status.textContent = "⏳ Lade Marktdaten...";
    content.innerHTML = "";

    try {
        const response = await fetch("https://api.opsucht.net/market/prices");
        const data = await response.json();

        for (const category in data) {
            const categoryTitle = document.createElement("h2");
            categoryTitle.textContent = category;
            content.appendChild(categoryTitle);

            const table = document.createElement("table");
            table.innerHTML = `
                <thead>
                    <tr>
                        <th>Item</th>
                        <th>BUY Preis</th>
                        <th>BUY Orders</th>
                        <th>SELL Preis</th>
                        <th>SELL Orders</th>
                    </tr>
                </thead>
                <tbody></tbody>
            `;

            const tbody = table.querySelector("tbody");

            for (const item in data[category]) {
                const orders = data[category][item];

                const buy = orders.find(o => o.orderSide === "BUY") || {};
                const sell = orders.find(o => o.orderSide === "SELL") || {};

                const row = document.createElement("tr");
                row.innerHTML = `
                    <td>${item}</td>
                    <td class="buy">${buy.price ?? "-"}</td>
                    <td>${buy.activeOrders ?? "-"}</td>
                    <td class="sell">${sell.price ?? "-"}</td>
                    <td>${sell.activeOrders ?? "-"}</td>
                `;
                tbody.appendChild(row);
            }

            content.appendChild(table);
        }

        status.textContent = "✅ Marktdaten erfolgreich geladen";

    } catch (e) {
        console.error(e);
        status.textContent = "❌ Fehler beim Laden der Marktdaten";
    }
}
</script>

</body>
</html>
