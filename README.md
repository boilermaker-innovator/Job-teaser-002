# Job-teaser-002<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Job Teaser Generator</title>
    <style>
        body { font-family: Arial, sans-serif; max-width: 800px; margin: 0 auto; padding: 20px; }
        input, button { font-size: 16px; padding: 10px; margin: 10px 0; }
        #teaserResult { margin-top: 20px; border: 1px solid #ddd; padding: 10px; }
    </style>
</head>
<body>
    <h1>Job Teaser Generator</h1>
    <input type="text" id="jobUrl" placeholder="Paste job ad URL here">
    <button onclick="generateTeaser()">Generate Teaser</button>
    <div id="teaserResult"></div>

    <script>
        function generateTeaser() {
            var url = document.getElementById('jobUrl').value;
            var result = "This is a teaser for the job at: " + url;
            document.getElementById('teaserResult').innerHTML = result;
        }
    </script>
</body>
</html>
