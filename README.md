# Wichtig
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Umfrage: Wer liebt mehr?</title>
    <script>
        function checkAnswer() {
            const selectedAnswer = document.querySelector('input[name="answer"]:checked').value;
            if (selectedAnswer === "Nein") {
                alert("Das war die falsche Antwort");
            } else {
                alert("Danke für deine Antwort!");
            }
        }
    </script>
</head>
<body>
    <h1>Umfrage: Wer liebt mehr, Tizian oder Mia?</h1>
    <form>
        <label>
            <input type="radio" name="answer" value="Ja" required> Ja
        </label><br>
        <label>
            <input type="radio" name="answer" value="Nein"> Nein
        </label><br><br>
        <button type="button" onclick="checkAnswer()">Antwort absenden</button>
    </form>
</body>
</html>
