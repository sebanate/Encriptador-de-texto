<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Text Encryptor</title>
</head>
<body>
    <h1>Text Encryptor</h1>
    <textarea id="inputText" rows="4" cols="50" placeholder="Enter text to encrypt..."></textarea>
    <br>
    <button onclick="encryptText()">Encrypt</button>
    <h2>Encrypted Text</h2>
    <textarea id="encryptedText" rows="4" cols="50" readonly></textarea>

    <script>
        function encryptText() {
            const text = document.getElementById('inputText').value;
            const encrypted = btoa(text); // Simple base64 encoding
            document.getElementById('encryptedText').value = encrypted;
        }
    </script>
</body>
</html>
# Encriptador-de-texto
