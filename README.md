# Responsive Web Design Certification
In this Responsive Web Design Certification, you will learn the languages developers use to create webpages: HTML (Hypertext Markup Language) for content and CSS (Cascading Style Sheets) for design.

To start, you'll master the fundamentals of HTML and CSS by creating a cat photo app. Eventually, you will construct a penguin to learn about current approaches like CSS variables, and a quiz site to learn about the best standards for accessibility.

Lastly, you will learn how to create responsive webpages using CSS Grid to create a magazine article layout and Flexbox to build a photo gallery.

`index.html`

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Survey Form</title>
</head>
<body>
    <h1 id="title">MancsAlgo Survey Form</h1>
    <p id="description">Thank you for taking the time to help us improve the platform!</p>
    <form action="" id="survey-form">
        <fieldset>
            <legend>Your Information</legend>
            <label for="" id="name-label">Enter Your Name: <input type="text" id="name" placeholder="Enter Your Name" required></label>
        <label for="" id="email-label">Your Email: <input type="email" id="email" placeholder="Enter Your Email" required></label>
        <label for="" id="number-label">Your Age: <input type="number" id="number" min="13" max="100" placeholder="Age"></label>
        <label for="dropdown"> How did you know about us?
            <select id="dropdown">
                <option value="">Others</option>
                <option value="">Facebook</option>
                <option value="">Youtube</option>
                <option value="">Website Ads</option>
            </select>
        </label>
        </fieldset>
        <fieldset>
            <legend>Do you have any experience in programming?</legend>
            <label for="experience"><input class="inline" type="radio" name="experience" id="experience" value="yes" checked>  Yes</label>
            <label for="experience"><input class="inline" type="radio" name="experience" id="experience" value="no"> No</label>
        </fieldset>
        <fieldset>
            <legend>What languages do you know?</legend>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="C"> C</label>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="C++"> C++</label>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="Java"> Java</label>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="Javascript"> Python</label>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="Javascript"> C#</label>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="Javascript"> Lua</label>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="Javascript"> Arduino</label>
            <label for="languages"><input class="inline" type="checkbox" name="languages" id="languages" value="Javascript"> Javascript</label>
        </fieldset>
        <fieldset>
            <legend>Please Leave us a message</legend>
            <label for="message"><textarea name="message" id="message" cols="70" rows="10"></textarea></label>
        </fieldset>
        <input type="submit" value="Submit" id="submit">
    </form>
</body>
</html>
```

`styles.css`

```
* {
    font-family: Tahoma, sans-serif;
}

body {
    width: 100%;
    height: 100vh;
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7;
}

#title, p {
    margin: 1em auto;
    text-align: center;
}

label {
    display: block;
    margin: 0.5rem 0;
    font-size: 16px;
}

input {
  width: 100%;
}

.inline {
    width: unset;
    margin: 0 0.5em 0 0;
    vertical-align: middle;
}
```
