# Python-Test
from flask import Flask
app = Flask(__name__)

html_code = """
<!DOCTYPE html>
<html>
<head>
    <title>My Python Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: #f0f0f0;
            text-align: center;
            padding: 50px;
        }
        h1 {
            color: #2c3e50;
        }
        p {
            font-size: 18px;
            color: #555;
        }
        .box {
            background: white;
            padding: 30px;
            margin: auto;
            border-radius: 10px;
            width: 80%;
            max-width: 600px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body>
    <div class="box">
        <h1>Welcome to My Python Website!</h1>
        <p>This is a simple website built with <strong>Python + Flask</strong>.</p>
        <p>Created by: <b>SHAREA SOBUJ</b></p>
    </div>
</body>
</html>
"""

@app.route('/')
def home():
    return html_code

if __name__ == '__main__':
    app.run(debug=True)
    
