# flip-cards
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>ford flashcards</title>
<style>
body {
font-family: 'Arial', sans-serif;
background-color: #f0f4f8;
margin: 0;
padding: 20px;
}

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
.card-container {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
gap: 20px;
max-width: 1000px;
margin: 0 auto;
}
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
.card:hover {
transform: translateY(-5px);
box-shadow: 0 8px 16px rgba(0,0,0,0.2);
}
.question {
font-weight: bold;
font-size: 1.2em;
text-align: center;
}
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
.card:hover .answer {
transform: translateY(0);
opacity: 1;
}
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
<div class="question">What car was the most sold in 1930?</div>
<div class="answer"><p>ford model A</p></div>
</div>
<!-- Card 2 -->
<div class="card">
<div class="question">when did the model A enter production?</div>
<div class="answer"><p>1927</p></div>
</div>
<!-- Card 3 -->
<div class="card">
<div class="question">what was henrry fords firs car he built.</div>
<div class="answer"><p>a simple quadracycle in 1996</p></div>
</div>
<!-- Card 4 -->
<div class="card">
<div class="question">what was henry ford first factorys name.</div>
<div class="answer"><p>Ford Piquette Avenue Plant</p></div>
</div>
<!-- Card 5 -->
<div class="card">
<div class="question">how many model A's were produced over the course of there production</div>
<div class="answer"><p>4.85 million</p></div>
</div>
<!-- Card 6 -->
<div class="card">
<div class="question">what was the ford motor companys most sucesfull car ever</div>
<div class="answer"><p>Ford F-Series pickup</p></div>
</div>
<!-- Card 7 -->
<div class="card">
<div class="question">at peak production how many model A's were made per day.</div>
<div class="answer"><p>9000</p></div>
</div>
<!-- Card 8 -->
<div class="card">
<div class="question">how much did  model a cost when new.</div>
<div class="answer"><p>four to six hundred dollors.</p></div>
</div>
</div>

</body>
</html>
