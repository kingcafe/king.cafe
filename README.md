<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>King Cafe</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #333;
            text-align: center;
            padding: 20px;
        }

        header h1 {
            color: gold;
            margin: 0;
        }

        nav {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            background-color: #444;
        }

        nav button {
            background-color: #444;
            color: white;
            border: none;
            padding: 15px 20px;
            cursor: pointer;
            font-size: 16px;
            flex: 1 1 auto;
            min-width: 120px;
            transition: background-color 0.3s, color 0.3s;
        }

        nav button:hover {
            background-color: #666;
        }

        nav button.active {
            background-color: gold;
            color: black;
            font-weight: bold;
        }

        .section {
            display: none;
            padding: 20px;
            background-size: cover;
            background-position: center;
            color: #fff;
            min-height: 300px;
        }

        .active {
            display: block;
        }

        ul {
            list-style: none;
            padding: 0;
        }

        ul li {
            margin: 10px 0;
            font-size: 18px;
        }

        @media (max-width: 600px) {
            nav {
                flex-direction: column;
            }

            nav button {
                font-size: 18px;
                padding: 15px;
            }

            ul li {
                font-size: 16px;
            }

            .section {
                padding: 15px;
            }

            header {
                font-size: 20px;
                padding: 15px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>King Cafe</h1>
    </header>

    <nav>
        <button onclick="showSection(0)" class="active">نێرگەلەکان</button>
        <button onclick="showSection(1)">خواردن</button>
        <button onclick="showSection(2)">Section 3</button>
        <button onclick="showSection(3)">Section 4</button>
        <button onclick="showSection(4)">Section 5</button>
        <button onclick="showSection(5)">Section 6</button>
        <button onclick="showSection(6)">Section 7</button>
    </nav>

    <div id="sections">
        <div class="section active" style="background-image: url('nn.jpg');">
            <h2>تامەکان</h2>
            <ul>
                <li>King 1</li><li>King 2</li><li>King 3</li><li>King 4</li>
                <li>King 5</li><li>King 6</li><li>King 7</li><li>King 8</li>
                <li>King 9</li><li>King 10</li><li>King 11</li><li>Dw Sew</li>
                <li>بنیشت</li><li>بغدادی</li><li>کاسترۆ</li><li>لیمۆ</li>
            </ul>
            
      <h2>فرێشەکان</h2>
      <ul style="position: relative;">
        <li>سندی</li><li>ئەنەناس</li><li>فرێش vip</li>
       
    
      </ul>
        </div>

        <div class="section" style="background-image: url('your-image2.jpg');">
            <h2>خواردن</h2>
            <ul>
                <li>٤٠٠٠،٦٠٠٠،٨٠٠٠،١٠٠٠٠پیزا</li>
                <li>King 2</li><li>King 3</li><li>King 4</li><li>King 5</li>
                <li>King 6</li><li>King 7</li><li>King 8</li><li>King 9</li>
                <li>King 10</li><li>King 11</li><li>Dw Sew</li>
                <li>بنیشت</li><li>بغدادی</li><li>کاسترۆ</li><li>لیمۆ</li>
            </ul>
        </div>

        <div class="section" style="background-image: url('your-image3.jpg');">
            <h2>Section 3</h2>
            <ul><li>1</li><li>2</li><li>3</li><li>4</li><li>5</li><li>6</li><li>7</li><li>8</li><li>9</li></ul>
        </div>

        <div class="section" style="background-image: url('your-image4.jpg');">
            <h2>Section 4</h2>
            <ul><li>1</li><li>2</li><li>3</li><li>4</li><li>5</li><li>6</li><li>7</li><li>8</li><li>9</li></ul>
        </div>

        <div class="section" style="background-image: url('your-image5.jpg');">
            <h2>Section 5</h2>
            <ul><li>1</li><li>2</li><li>3</li><li>4</li><li>5</li><li>6</li><li>7</li><li>8</li><li>9</li></ul>
        </div>

        <div class="section" style="background-image: url('your-image6.jpg');">
            <h2>Section 6</h2>
            <ul><li>1</li><li>2</li><li>3</li><li>4</li><li>5</li><li>6</li><li>7</li><li>8</li><li>9</li></ul>
        </div>

        <div class="section" style="background-image: url('your-image7.jpg');">
            <h2>Section 7</h2>
            <ul><li>1</li><li>2</li><li>3</li><li>4</li><li>5</li><li>6</li><li>7</li><li>8</li><li>9</li></ul>
        </div>
    </div>

    <script>
        function showSection(index) {
            const sections = document.querySelectorAll('.section');
            const buttons = document.querySelectorAll('nav button');

            sections.forEach((section, i) => {
                section.classList.toggle('active', i === index);
            });

            buttons.forEach((btn, i) => {
                btn.classList.toggle('active', i === index);
            });
        }
    </script>
</body>
</html>
