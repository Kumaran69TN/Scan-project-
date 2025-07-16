<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>QR Scan & Count - Muthu Kumaran</title>
  <script src="https://unpkg.com/html5-qrcode"></script>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #e0f7fa;
      text-align: center;
      padding: 20px;
    }
    h1 {
      color: #006064;
      font-size: 24px;
    }
    #countDisplay {
      font-size: 20px;
      margin: 20px 0;
      color: #004d40;
    }
    #reader {
      width: 100%;
      max-width: 320px;
      margin: auto;
    }
    button {
      padding: 12px 24px;
      font-size: 16px;
      margin: 10px;
      border: none;
      background: #00796b;
      color: white;
      border-radius: 8px;
    }
    button:active {
      background-color: #004d40;
    }
  </style>
</head>
<body>

  <h1>📦 QR Scanner - Muthu Kumaran</h1>

  <div id="countDisplay">Scanned: <span id="count">0</span> / 100</div>

  <div id="reader"></div>

  <button onclick="resetCount()">🔄 Reset</button>

  <script>
    let count = parseInt(localStorage.getItem('scanCount')) || 0;
    let scannedItems = JSON.parse(localStorage.getItem('scannedItems')) || [];

    document.getElementById("count").innerText = count;

    function onScanSuccess(decodedText, decodedResult) {
      if (!scannedItems.includes(decodedText)) {
        scannedItems.push(decodedText);
        count++;
        localStorage.setItem('scanCount', count);
        localStorage.setItem('scannedItems', JSON.stringify(scannedItems));
        document.getElementById("count").innerText = count;
        alert("✅ Scanned: " + decodedText);
      } else {
        alert("⚠️ Already scanned: " + decodedText);
      }
    }

    function resetCount() {
      if (confirm("Sure to reset everything?")) {
        count = 0;
        scannedItems = [];
        localStorage.setItem('scanCount', 0);
        localStorage.setItem('scannedItems', JSON.stringify([]));
        document.getElementById("count").innerText = 0;
      }
    }

    const html5QrCode = new Html5Qrcode("reader");
    Html5Qrcode.getCameras().then(cameras => {
      if (cameras && cameras.length) {
        html5QrCode.start(
          { facingMode: "environment" },
          {
            fps: 10,
            qrbox: { width: 250, height: 250 }
          },
          onScanSuccess
        );
      } else {
        alert("No camera found!");
      }
    }).catch(err => {
      alert("Camera error: " + err);
    });
  </script>

</body>
</html>
