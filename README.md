<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página de Pagos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 400px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .payment-option {
            margin: 10px 0;
            padding: 10px;
            background: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            display: block;
            width: 100%;
        }
        .payment-option:hover {
            background: #0056b3;
        }
        .payment-info {
            margin: 5px 0;
            font-size: 14px;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Realizar Pago</h2>
        <button class="payment-option" onclick="payWithMetaMask()">Pagar con MetaMask</button>
        <p class="payment-info">MetaMask: 0xf88c17b82e3f4ec537fc89713939100efc112005</p>
        <button class="payment-option" onclick="copyToClipboard('0xf88c17b82e3f4ec537fc89713939100efc112005')">Copiar MetaMask</button>
        <p class="payment-info">Plim: 917817909</p>
        <button class="payment-option" onclick="copyToClipboard('917817909')">Copiar Plim</button>
        <p class="payment-info">Yape: 930287493</p>
        <button class="payment-option" onclick="copyToClipboard('930287493')">Copiar Yape</button>
        <p class="payment-info">Plin: +51917817909</p>
        <button class="payment-option" onclick="copyToClipboard('+51917817909')">Copiar Plin</button>
        <p class="payment-info">Binance: TUfoP3fusXTsByBXwDmScwNwCBCqBCSxxq</p>
        <button class="payment-option" onclick="copyToClipboard('TUfoP3fusXTsByBXwDmScwNwCBCqBCSxxq')">Copiar Binance</button>
        <p class="payment-info">BCP Cuenta: 19205743039048</p>
        <button class="payment-option" onclick="copyToClipboard('19205743039048')">Copiar BCP Cuenta</button>
        <p class="payment-info">BCP CCI: 00219210574303904833</p>
        <button class="payment-option" onclick="copyToClipboard('00219210574303904833')">Copiar BCP CCI</button>
        <p class="payment-info">BBVA Cuenta: 0011-0579-0234133852</p>
        <button class="payment-option" onclick="copyToClipboard('0011-0579-0234133852')">Copiar BBVA Cuenta</button>
        <p class="payment-info">BBVA CCI: 01157900023413385209</p>
        <button class="payment-option" onclick="copyToClipboard('01157900023413385209')">Copiar BBVA CCI</button>
        <p class="payment-info">PayPal: <a href="https://www.paypal.com/invoice/p/#Y6MTREEM3C9AB6BY" target="_blank">Realizar Pago</a></p>
    </div>
    
    <script>
        function payWithMetaMask() {
            alert('Redirigiendo a MetaMask...');
            // Aquí podrías integrar MetaMask si es necesario.
        }
        
        function copyToClipboard(text) {
            navigator.clipboard.writeText(text).then(() => {
                alert('Copiado al portapapeles: ' + text);
            }).catch(err => {
                console.error('Error al copiar', err);
            });
        }
    </script>
</body>
</html>
