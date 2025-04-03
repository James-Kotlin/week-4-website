# week-4-website
week 4 website assignment

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Webpage</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #4CAF50;
            color: white;
            padding: 1rem;
            text-align: center;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            padding: 1rem;
        }

        .box {
            flex: 1 1 calc(33.33% - 1rem);
            margin: 0.5rem;
            background-color: #f4f4f4;
            border: 1px solid #ccc;
            text-align: center;
            padding: 1rem;
        }

        .grid-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            padding: 1rem;
        }

        .grid-item {
            background-color: #f4f4f4;
            border: 1px solid #ccc;
            text-align: center;
            padding: 1rem;
        }

        @media (max-width: 768px) {
            .box {
                flex: 1 1 calc(50% - 1rem);
            }

            .grid-container {
                grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            }
        }

        @media (max-width: 480px) {
            .box {
                flex: 1 1 100%;
            }

            .grid-container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Responsive Webpage</h1>
    </header>

    <section class="container">
        <div class="box">Box 1</div>
        <div class="box">Box 2</div>
        <div class="box">Box 3</div>
    </section>

    <section class="grid-container">
        <div class="grid-item">Grid Item 1</div>
        <div class="grid-item">Grid Item 2</div>
        <div class="grid-item">Grid Item 3</div>
        <div class="grid-item">Grid Item 4</div>
    </section>
</body>
</html>
