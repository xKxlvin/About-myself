<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yuji Itadori Waving Animation</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
        }

        .sprite {
            width: 100px; /* Width of a single frame */
            height: 100px; /* Height of a single frame */
            background: url('yuji_sprite.png') left center;
            background-size: cover;
            animation: wave 1s steps(10) infinite; /* Adjust steps(10) based on the number of frames */
        }

        @keyframes wave {
            from { background-position: 0; }
            to { background-position: -1000px; } /* Adjust based on the total width of the sprite sheet */
        }
    </style>
</head>
<body>
    <div class="sprite"></div>
</body>
</html>
