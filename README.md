# Static Website: Form a Story

Simple static website using HTTP forms and CSS styling.

## HTML: Home
```
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css?family=Open+Sans" rel="stylesheet">
    <title>Form a Story</title>
  </head>
  <body>
    <section id="top">
      <img src="https://content.codecademy.com/courses/learn-html-forms/formAStoryLogo.svg" alt="Form A Story Logo">
    </section>
    <section id="main">
      <h1>Complete the Form -<br> Complete the Story!</h1>
      <hr>
      <!--Add your form below:-->
      <form action="story.html" method="GET">
        <label for="animal-1">Animal:</label>
        <input type="text" id="animal-1" name="animal-1">
        <br>
        <label for="animal-2">Another Animal:</label>
        <input type="text" id="animal-2" required>
        <br>
        <label for="animal-3">One More Animal:</label>
        <input type="text" id="animal-3" required>
        <br>
        <label for="adj-1">Adjective (past tense):</label>
        <input type="text" id="adj-1">
        <br>
        <label for="verb-1">Verb (ends in -ing:</label>
        <input type="text" id="verb-1" required>
        <br>
        <label for="num-1">Number:</label>
        <input type="number" id="num-1" name="num-1" required>
        <br>
        <span>Yes or No:</span>
        <input id="yes" type="radio" name="answer" value="yes" required>
        <label for="yes">Yes</label>
        <input id="no" type="radio" name="answer" value="no" required>
        <label for="no">No</label>
        <br>
        <label>Relative speed (ends in -er):</label>
        <select id="speed" name="speed" required>
          <option value="slower">Slower</option>
          <option value="slow">Slow</option>
          <option value="fast">Fast</option>
          <option value="faster">Faster</option>
        </select>
        <br>
        <label for="quote"> Motivational Quote:</label>
          <input id="quote" name="quote" type="text" required list="quote-choices">
            <datalist id="quote-choices">
              <option value="winner gets ice cream!"></option>
              <option value="I'm a super billionaire"></option>
              <option value="Hacked the life out of it"></option>
              <option value="Yessir"></option>
            </datalist>
        <br>
          <label for="message">Meaningful Message:</label>
            <textarea id="message" name="message" row="8" cols="40" required></textarea>
        <br>
        <input type="submit" value="Form My Story!">
      </form>
    </section>
  </body>
</html>
```

## HTML: Original
```
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Completed Story</title>
    <script type="text/javascript" src="main.js" defer></script>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <section id="top">
      <img src="https://content.codecademy.com/courses/learn-html-forms/formAStoryLogo.svg" alt="Form A Story Logo">
    </section>
    <section id="main">
      <h1 id="title">The Tortoise and the Hare</h1>
      <article id="story">
        <p>A Hare was making fun of the Tortoise one day for being so slow.</p>

        <p>"Do you ever get anywhere?" he asked with a mocking laugh.</p>

        <p>"Yes," replied the Tortoise, "and I get there sooner than you think. I'll run you a race and prove it."</p>

        <p>The Hare was much amused at the idea of running a race with the Tortoise, but for the fun of the thing he agreed. So the Fox, who had consented to act as judge, marked the distance and started the runners off.</p>

        <p>The Hare was soon far out of sight, and to make the Tortoise feel very deeply how ridiculous it was for him to try a race with a Hare, he lay down beside the course to take a nap until the Tortoise should catch up.</p>

        <p>The Tortoise meanwhile kept going slowly but steadily, and, after a time, passed the place where the Hare was sleeping. But the Hare slept on very peacefully; and when at last he did wake up, the Tortoise was near the goal. The Hare now ran his swiftest, but he could not overtake the Tortoise in time.</p>
      </article>

      <hr>
     <a href="index.html">Start Over!</a>
    </section>

  </body>
</html>
```

## HTML: Story
```
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Completed Story</title>
    <script type="text/javascript" src="main.js" defer></script>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <section id="top">
      <img src="https://content.codecademy.com/courses/learn-html-forms/formAStoryLogo.svg" alt="Form A Story Logo">
    </section>
    <section id="main">
      <h1 id="title"></h1>
      <article id="story"></article>
      <h2 id="moral">Moral of the story:</h2>
      <article id="moral-message"></article>
      <hr>
      <a href="index.html">Start Over!</a>
      <span> || </span>
      <a href="original.html">Original Story</a>
    </section>

  </body>
</html>
```

## CSS

```
body {
    background-color: rgb(255, 199, 64);
    font-family: "Open Sans", Arial;
  }
  
  form {
    line-height: 27px;
  }
  
  h2 {
    font-size: 20px;
  }
  
  input[type="text"], input[type="number"] {
    min-height: 15px;
    border-radius: 5px;
    border:1px solid #cccccc;
  }
  
  input[type="radio"] {
    margin-left: 12px;
  }
  
  #main {
    background-color: rgba(255,255,255,0.8);
    text-align: center;
    height: 80vh;
    border-radius: 15px;
    margin: 2% 10%;
    overflow: auto;
  }
  
  #story {
    padding: 0 3%;
  }
  
  #top {
    background-color: rgb(255, 255, 255);
    margin: 2% 10%;
    border-radius: 15px;
  }
  
  #top img {
    display: block;
    width: 35%;
    margin: 0 auto;
  }
  
  .italics {
    font-style: italic;
  }
  
  .word {
    font-weight: bold;
    text-decoration: underline;
  }
```
