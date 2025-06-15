# Review-Cards-Assignment
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>French Class Flashcards</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f0f8ff;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    h1 {
      margin: 30px 0;
      font-size: 2.5rem;
      color: #333;
      animation: slideDown 1s ease-out;
    }

    @keyframes slideDown {
      from {
        transform: translateY(-100px);
        opacity: 0;
      }
      to {
        transform: translateY(0);
        opacity: 1;
      }
    }

    .card-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      padding: 20px;
      max-width: 1000px;
      width: 100%;
    }

    .card {
      position: relative;
      background: #ffffff;
      border: 2px solid #ccc;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease;
      cursor: pointer;
      overflow: hidden;
    }

    .card:hover {
      transform: scale(1.05);
    }

    .question {
      font-weight: bold;
      font-size: 1.1rem;
      color: #333;
    }

    .answer {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      padding: 15px;
      background-color: #e0f7fa;
      color: #000;
      text-align: center;
      opacity: 0;
      transform: translateY(100%);
      transition: transform 0.5s ease, opacity 0.5s ease;
      border-top: 2px solid #00796b;
    }

    .card:hover .answer {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body>
  <h1>French Vocabulary Review</h1>
  <div class="card-container">
    <div class="card">
      <div class="question">What is "to eat lunch" in French?</div>
      <div class="answer">déjeuner</div>
    </div>
    <div class="card">
      <div class="question">How do you say "4:00 PM" in French?</div>
      <div class="answer">Il est seize heures</div>
    </div>
    <div class="card">
      <div class="question">Translate: "We talk"</div>
      <div class="answer">Nous parlons</div>
    </div>
    <div class="card">
      <div class="question">What is "art class" in French?</div>
      <div class="answer">les arts plastiques</div>
    </div>
    <div class="card">
      <div class="question">How do you say "to the right"?</div>
      <div class="answer">à droite</div>
    </div>
    <div class="card">
      <div class="question">Translate: "Je viens à l'école à huit heures."</div>
      <div class="answer">I come to school at 8:00.</div>
    </div>
    <div class="card">
      <div class="question">What is the French word for Chemistry?</div>
      <div class="answer">la chimie</div>
    </div>
    <div class="card">
      <div class="question">What does "le collège" mean?</div>
      <div class="answer">Middle school</div>
    </div>
  </div>
</body>
</html>
