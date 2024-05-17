# Learn HTML Forms by Building a Registration Form
HTML forms are a useful tool for gathering data from website visitors.

By creating a signup page, you will gain knowledge of HTML forms in this course. You'll discover new CSS style tools and how to restrict the kinds of data users can enter into your form.

`index.html`

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Form</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Registration Form</h1>
    <p>Please fill out this form with the required information</p>
    <form action="https://register-demo.freecodecamp.org" method="post">
        <fieldset>
            <label for="first-name">Enter Your First Name: <input name="first-name" id="first-name" type="text" required></label>
            <label for="last-name">Enter Your Last Name: <input name="last-name" id="last-name" type="text" required></label>
            <label for="email">Enter Your Email: <input name="email" id="email" type="email" required></label>
            <label for="new-password">Create a New Password: <input name="new-passwor" id="new-password" type="password" patter="[a-z0-5]{8,}" required></label>
        </fieldset>
        <fieldset>
            <legend>Account type (required)</legend>
            <label for="personal-account"><input type="radio" name="account-type" id="personal-account" checked class="inline"> Personal</label>
            <label for="business-account"><input type="radio" name="account-type" id="business-account" class="inline"> Business</label> 
        </fieldset>
        <fieldset>
            <label for="profile-picture">Upload a profile picture:  <input name="profile-picture" type="file" id="profile-picture"></label>
            <label for="age">Input your age (years): <input name="age" type="number" min="13" max="120" id="age"> </label>
            <label for="referrer"> How did you hear about us?
                <select name="referrer" id="referrer">
                    <option value="">(select one)</option>
                    <option value="1">freeCodeCamp News</option>
                    <option value="2">freeCodeCamp YouTube Channel</option>
                    <option value="3">freeCodeCamp Forum</option>
                    <option value="4">Other</option>
                </select>
            </label>
            <label for="bio"> Provide a bio: 
                <textarea name="bio" id="bio" rows="3" cols="30" placeholder="I like coding on the beach..."></textarea>
            </label>
        </fieldset>
        <label for="terms-and-conditions"><input name="terms-and-conditions" type="checkbox" id="terms-and-conditions" class="inline" required>I accept the <a href="https://www.freecodecamp.org/news/terms-of-service/">terms and conditions</a></label>
        <input type="submit" value="Submit">
    </form>
</body>
</html>
```

`styles.css`

```

body {
    width: 100%;
    height: 100vh;
    margin: 0;
    background-color: #1b1b32;
    color: #f5f6f7;
}

label {
    display: block;
    margin: 0.5rem 0;
    font-family: Tahoma, sans-serif;
    font-size: 16px;
}

h1, p {
    margin: 1em auto;
    text-align: center;
}

form {
    margin: 0 auto;
    max-width: 500px;
    min-width: 300px;
    width: 60vw;
    padding-bottom: 2em;
}

fieldset {
    border: 0;
    padding: 2rem 0;
    border-bottom: 3px solid #3b3b4f;
}

fieldset:last-of-type {
    border-bottom: none;
}

input, textarea, select {
    margin: 10px 0 0 ;
    width: 100%;
    min-height: 2em;
}

.inline {
    width: unset;
    margin: 0 0.5em 0 0;
    vertical-align: middle;
}

input, textarea {
    background-color: #0a0a23;
    border: 1px solid #0a0a23;
    color: #ffffff;
    
}

input[type="submit"]{
    display: block;
    width: 60%;
    height: 2em;
    margin: 0 auto;
    font-size: 1.1rem;
    background-color: #3b3b4f;
    border-color: white;
    min-width: 300px;
    margin: 1em auto;
}

input[type="file"]{
    padding: 1px 2px;
}

a {
    color: #dfdfe2;
}

```
