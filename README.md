# flip-cards
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Flashcard Review Activity</title>
<style>
/* Basic Reset and Styling */
body {
font-family: 'Arial', sans-serif;
background-color: #f0f4f8;
margin: 0;
padding: 20px;
}

/* Title with animation */
h1 {
text-align: center;
font-size: 2.5em;
margin-bottom: 30px;
opacity: 0;
animation: fadeIn 2s forwards;
}

@keyframes fadeIn {
from { opacity: 0; transform: translateY(-20px); }
to { opacity: 1; transform: translateY(0); }
}

/* Container for all cards */
.card-container {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
gap: 20px;
max-width: 1000px;
margin: 0 auto;
}

/* Individual card styling */
.card {
background-color: #ffffff;
border-radius: 10px;
box-shadow: 0 4px 8px rgba(0,0,0,0.1);
padding: 20px;
position: relative;
overflow: hidden;
cursor: pointer;
height: 150px;
display: flex;
flex-direction: column;
justify-content: center;
transition: transform 0.3s ease, box-shadow 0.3s ease;
}

/* Slight lift on hover */
.card:hover {
transform: translateY(-5px);
box-shadow: 0 8px 16px rgba(0,0,0,0.2);
}

/* Question/Term styling */
.question {
font-weight: bold;
font-size: 1.2em;
text-align: center;
}

/* Answer container */
.answer {
position: absolute;
bottom: 0;
left: 0;
right: 0;
background-color: #e0f7fa;
padding: 15px;
box-sizing: border-box;
transform: translateY(100%);
opacity: 0;
transition: transform 0.5s ease, opacity 0.5s ease;
border-top: 2px solid #0097a7;
border-radius: 0 0 10px 10px;
}

/* Reveal answer on hover */
.card:hover .answer {
transform: translateY(0);
opacity: 1;
}

/* Optional: Add some text styling inside answer */
.answer p {
margin: 0;
font-size: 1em;
color: #006064;
}
</style>
</head>
<body>

<h1>Flashcard Review Activity</h1>

<div class="card-container">
<!-- Card 1 -->
<div class="card">
<div class="question">What is the capital of France?</div>
<div class="answer"><p>Paris</p></div>
</div>
<!-- Card 2 -->
<div class="card">
<div class="question">Who developed the theory of relativity?</div>
<div class="answer"><p>Albert Einstein</p></div>
</div>
<!-- Card 3 -->
<div class="card">
<div class="question">What is the chemical symbol for Gold?</div>
<div class="answer"><p>Au</p></div>
</div>
<!-- Card 4 -->
<div class="card">
<div class="question">Name the process by which plants make food.</div>
<div class="answer"><p>Photosynthesis</p></div>
</div>
<!-- Card 5 -->
<div class="card">
<div class="question">Who was the first President of the United States?</div>
<div class="answer"><p>George Washington</p></div>
</div>
<!-- Card 6 -->
<div class="card">
<div class="question">What is the largest planet in our Solar System?</div>
<div class="answer"><p>Jupiter</p></div>
</div>
<!-- Card 7 -->
<div class="card">
<div class="question">What language is primarily spoken in Brazil?</div>
<div class="answer"><p>Portuguese</p></div>
</div>
<!-- Card 8 -->
<div class="card">
<div class="question">What is the boiling point of water?</div>
<div class="answer"><p>100°C (212°F) at sea level</p></div>
</div>
</div>

</body>
</html>
