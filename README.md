# Survey-Form-

Solution for Build a Survey Form
Close
×
HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Survey Form | New Foundation Academy</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="container">
    <h1 id="title">New Foundation Academy Survey</h1>
    <p id="description">We value your feedback. Please take a moment to fill out this survey.</p>

    <form id="survey-form">
      <!-- Name Field -->
      <label id="name-label" for="name">Name:</label>
      <input type="text" id="name" name="name" placeholder="Enter your name" required>

      <!-- Email Field -->
      <label id="email-label" for="email">Email:</label>
      <input type="email" id="email" name="email" placeholder="Enter your email" required>

      <!-- Age Field -->
      <label id="number-label" for="number">Age:</label>
      <input type="number" id="number" name="age" min="1" max="120" placeholder="Enter your age" required>

      <!-- Dropdown Field -->
      <label for="dropdown">Which category best describes you?</label>
      <select id="dropdown" name="role">
        <option value="" disabled selected>Select an option</option>
        <option value="student">Student</option>
        <option value="teacher">Teacher</option>
        <option value="parent">Parent</option>
      </select>

      <!-- Radio Buttons -->
      <p>How would you rate your overall experience?</p>
      <label><input type="radio" name="experience" value="excellent"> Excellent</label>
      <label><input type="radio" name="experience" value="good"> Good</label>
      <label><input type="radio" name="experience" value="fair"> Fair</label>

      <!-- Checkboxes -->
      <p>Which services did you find useful? (Check all that apply)</p>
      <label><input type="checkbox" name="services" value="library"> Library</label>
      <label><input type="checkbox" name="services" value="cafeteria"> Cafeteria</label>
      <label><input type="checkbox" name="services" value="sports"> Sports</label>

      <!-- Textarea -->
      <label for="comments">Any additional comments:</label>
      <textarea id="comments" name="comments" placeholder="Enter your comments here..."></textarea>

      <!-- Submit Button -->
      <button id="submit" type="submit">Submit</button>
    </form>
  </div>
</body>
</html>
CSS
body {
  width: 100%;
  height: 100vh;
  margin: 0;
  background-color: #1b1b32;
  color: #f5f6f7;
  font-family: Tahoma;
  font-size: 16px;
}

h1, p {
  margin: 1em auto;
  text-align: center;
}

form {
  width: 60vw;
  max-width: 500px;
  min-width: 300px;
  margin: 0 auto;
  padding-bottom: 2em;
}

fieldset {
  border: none;
  padding: 2rem 0;
  border-bottom: 3px solid #3b3b4f;
}

fieldset:last-of-type {
  border-bottom: none;
}

label {
  display: block;
  margin: 0.5rem 0;
}

input,
textarea,
select {
  margin: 10px 0 0 0;
  width: 100%;
  min-height: 2em;
}

input, textarea {
  background-color: #0a0a23;
  border: 1px solid #0a0a23;
  color: #ffffff;
}

.inline {
  width: unset;
  margin: 0 0.5em 0 0;
  vertical-align: middle;
}

input[type="submit"] {
  display: block;
  width: 60%;
  margin: 1em auto;
  height: 2em;
  font-size: 1.1rem;
  background-color: #3b3b4f;
  border-color: white;
  min-width: 300px;
}

input[type="file"] {
  padding: 1px 2px;
}

.inline{
  display: inline; 
}

a{ color:#dfdfe2;}
Close
