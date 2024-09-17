<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exclusive Event: Get Free Bitcoin!</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f4f7fa;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 700px;
            margin: auto;
            background: #ffffff;
            padding: 30px;
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            border-top: 4px solid #ffcc00; /* Top border for a bold touch */
        }
        h1 {
            color: #ffcc00;
            font-size: 2.5em;
            margin-bottom: 15px;
            text-align: center;
        }
        h2 {
            color: #333333;
            margin-top: 20px;
            margin-bottom: 10px;
            font-weight: 700;
        }
        p {
            color: #555555;
            line-height: 1.7;
        }
        .fake-ad {
            border: 1px solid #ffcc00;
            padding: 20px;
            margin: 20px 0;
            border-radius: 8px;
            background: #fff8e1; /* Light yellow background */
        }
        .progress-container {
            margin: 20px 0;
            background: #eceff1;
            border-radius: 5px;
            position: relative;
        }
        .progress {
            background-color: #ffcc00;
            height: 25px;
            border-radius: 5px;
        }
        .copy-button {
            padding: 10px 15px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s; 
            margin-top: 10px;
            outline: none;
            text-align: center;
            display: inline-block;
        }
        .copy-button:hover {
            background-color: #0056b3;
        }
        .footer {
            margin-top: 30px;
            font-size: 0.9em;
            color: grey;
            text-align: center;
        }
        .share-buttons {
            margin-top: 20px;
            text-align: center;
        }
        .share-buttons a {
            margin: 5px;
            padding: 12px 18px;
            background-color: #ffcc00;
            color: white;
            text-decoration: none;
            border-radius: 25px;
            transition: background-color 0.3s, transform 0.3s;
            font-weight: bold;
        }
        .share-buttons a:hover {
            background-color: #e6b800;
            transform: scale(1.05); /* Slightly enlarge on hover */
        }
        .icon {
            vertical-align: middle;
            margin-right: 8px;
        }
        .separator {
            border-top: 1px solid #ccc;
            margin: 20px 0;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>🎉 Get Free Bitcoin Event!</h1>
    <p>Join our exclusive event! Send <strong>10 USDT</strong> for a chance to receive <strong>1 Bitcoin</strong> or send <strong>100 USDT</strong> to increase your chances of getting <strong>1 Bitcoin</strong>! Don't miss this incredible opportunity!</p>
    
    <div class="fake-ad">
        <h2>How to Participate:</h2>
        <ol>
            <li>Send the required amount to the address below:</li>
            <p>
                <strong>Address:</strong> <code id="btc-address">0x1b13286d3ae60040826441c096dfbd150e1c78d5</code>
                <button class="copy-button" onclick="copyAddress()">Copy Address</button>
            </p>
            <li>Comment below with your transaction ID for verification.</li>
            <li>Share this event with your friends to spread the word!</li>
        </ol>
        <h2>Current Participation Status:</h2>
        <div class="progress-container">
            <div class="progress" style="width: calc(156 / 300 * 100%);"></div>
        </div>
        <p><strong>Spots Taken:</strong> <span id="spots-taken">156</span> out of 300</p>
        <p><strong>Spots Left:</strong> <span id="spots-left">144</span></p>
    </div>

    <div class="separator"></div>
    
    <div class="share-buttons">
        <p><strong>Spread the Word:</strong></p>
        <a href="https://twitter.com/intent/tweet?text=Join+the+exclusive+event+to+get+free+Bitcoin!&url=https://example.com" target="_blank">
            <img class="icon" src="https://img.icons8.com/material-outlined/24/ffffff/twitter.png" alt="Twitter icon"/>
            Share on Twitter
        </a>
        <a href="https://www.facebook.com/sharer/sharer.php?u=https://example.com" target="_blank">
            <img class="icon" src="https://img.icons8.com/material-outlined/24/ffffff/facebook-new.png" alt="Facebook icon"/>
            Share on Facebook
        </a>
    </div>

    <div class="footer">
        
    </div>
</div>

<script>
    // JavaScript to dynamically update the number of spots taken and left
    const totalSpots = 300;
    const spotsTaken = 156; // Update this according to your requirements
    const spotsLeft = totalSpots - spotsTaken;
    document.getElementById('spots-taken').textContent = spotsTaken;
    document.getElementById('spots-left').textContent = spotsLeft;

    // Function to copy the address to clipboard
    function copyAddress() {
        const addressText = document.getElementById('btc-address').innerText;
        navigator.clipboard.writeText(addressText).then(() => {
            alert('Address copied to clipboard!'); // Alert user that the address was copied
        }).catch(err => {
            console.error('Failed to copy: ', err);
        });
    }
</script>

</body>
</html>
