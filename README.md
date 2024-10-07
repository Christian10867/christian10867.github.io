<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>STATION HOPE HORIZON</title>
    <style>
        body {
            background-color: #003300; /* Dark green background */
            color: #00ff00; /* Bright green text */
            font-family: 'Courier New', Courier, monospace; /* Monospace font */
            font-size: 16px;
            line-height: 1.5;
            margin: 0;
            padding: 20px;
            text-shadow: 0 0 5px #00ff00; /* Glow effect */
        }
        a {
            color: #00ff00;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        .terminal {
            max-width: 800px;
            margin: auto;
            white-space: pre-wrap; /* Preserve whitespace */
        }
        .scanlines {
            pointer-events: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(
                rgba(0, 0, 0, 0.1) 50%,
                transparent 50%
            );
            background-size: 100% 2px;
        }
        @keyframes blink {
            0% { opacity: 1; }
            50% { opacity: 0; }
            100% { opacity: 1; }
        }
        .cursor {
            display: inline-block;
            width: 10px;
            background-color: #00ff00;
            animation: blink 1s step-start infinite;
        }
        .link-list li {
            margin-left: 1.5em;      /* Adjust as needed */
            text-indent: -1.5em;     /* Negative of margin-left */
            list-style: none;        /* Remove default bullets */
        }
        .link-list li::before {
            content: '- ';           /* Add hyphen before each item */
        }
    </style>
</head>
<body>
    <div class="terminal">

           __                   __ _  __          ___
        /\ \ \_____  ____ _    / /(_)/ _| ___    / __\___  _ __ _ __
       /  \/ / _ \ \/ / _` |  / / | | |_ / _ \  / /  / _ \| '__| '_ \
      / /\  /  __/>  < (_| | / /__| |  _|  __/ / /__| (_) | |  | |_) |
      \_\ \/ \___/_/\_\__,_| \____/_|_|  \___| \____/\___/|_|  | .__(_)
                                                               |_|
        <p>STATION HOPE HORIZON - TERMINALS<p>

- <a href="Terminal_Dock_Main.html">Start Dock Terminal</a>
- <a href="Terminal_Medbay_Main.html">Start Medbay Terminal</a>

        <p>&gt; <span class="cursor"></span></p>
    </div>
    <div class="scanlines"></div>
</body>
</html>
