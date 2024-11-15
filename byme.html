<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Upload File</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            text-align: center;
            padding: 20px;
        }
        .container {
            background-color: white;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            width: 400px;
            margin: 0 auto;
        }
        h1 {
            color: #333;
        }
        input[type="file"] {
            margin: 20px 0;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
        }
        button:hover {
            background-color: #45a049;
        }
        .footer {
            margin-top: 20px;
            font-size: 14px;
            color: #777;
        }
        .banner {
            max-width: 100%;
            height: auto;
        }
    </style>
</head>
<body>

    <div class="container">
        <img class="banner" src="https://i.postimg.cc/wMVKzzRy/my-index.jpg" alt="Banner">
        <h1>Upload Your File</h1>
        <form id="uploadForm">
            <input type="file" name="file" id="file" required>
            <br>
            <button type="submit">Upload File</button>
        </form>
        <div id="response"></div>
    </div>

    <div class="footer">
        <p>DEV: SCREAM | <a href="https://discord.gg/UUUU" target="_blank">DISCORD</a></p>
    </div>

    <script>
        // Webhook URL for Discord
        const webhookURL = 'https://ptb.discord.com/api/webhooks/1306412272540712980/1ehx8cVVHGR2h9Md6kwrsyyLaJDtwwRxpF9nhvaL6lHOg-oBiQSbCoZpV9ACzk_gbK4F';

        // Function to send message to Discord via Webhook
        function sendToDiscord(message) {
            const payload = {
                content: message
            };

            fetch(webhookURL, {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify(payload)
            }).then(response => {
                if (response.ok) {
                    console.log("Message sent to Discord successfully.");
                } else {
                    console.error("Failed to send message to Discord.");
                }
            }).catch(error => {
                console.error("Error sending message to Discord:", error);
            });
        }

        document.getElementById('uploadForm').addEventListener('submit', function(event) {
            event.preventDefault();
            
            let formData = new FormData();
            formData.append('file', document.getElementById('file').files[0]);

            // Send notification that file upload started
            sendToDiscord("File upload started.");

            fetch('https://api.anonfiles.com/upload', {
                method: 'POST',
                body: formData
            })
            .then(response => response.json())
            .then(data => {
                if (data.fileUrl) {
                    const successMessage = `File uploaded successfully. Download link: ${data.fileUrl}`;
                    document.getElementById('response').innerHTML = `<p>${successMessage}</p>`;

                    // Send success notification to Discord
                    sendToDiscord(successMessage);
                } else {
                    const errorMessage = `Error: ${data.message}`;
                    document.getElementById('response').innerHTML = `<p>${errorMessage}</p>`;

                    // Send error notification to Discord
                    sendToDiscord(errorMessage);
                }
            })
            .catch(error => {
                const errorMessage = `Error: ${error}`;
                document.getElementById('response').innerHTML = `<p>${errorMessage}</p>`;

                // Send error notification to Discord
                sendToDiscord(errorMessage);
            });
        });
    </script>

</body>
</html>
