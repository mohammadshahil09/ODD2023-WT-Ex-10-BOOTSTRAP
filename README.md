# Ex-10-BOOTSTRAP
## AIM : To Develop programs to create attractive forms using Bootstrap
## Objective 1 : 
To Create a Responsive feedback form for a virtual workshop on Constructing Modern Websites built with Bootstrap.
## Procedure:
## Step 1:
Identify Form Fields:

Determine the necessary fields such as name, email, and feedback.
## Step 2:
Utilize Bootstrap Components:

Use Bootstrap classes (form-group, form-control, btn) for a responsive and visually appealing form layout.
## Step 3:
Implement Validation:

Add HTML5 validation attributes for required fields and email format.
## Step 4:
Customize Styling:

Adjust the form's appearance using Bootstrap utility classes or custom CSS.
## Step 5:
Test Responsiveness:

Ensure the form is responsive by testing it on various devices.
## Step 6:
Validate Form Submission:

Validate the form data on the server-side to ensure data integrity.

# Program:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Workshop Feedback Form</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

  <style>
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: linear-gradient(to right, #3498db, #1abc9c);
        color: #fff;
        margin: 0;
        padding: 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        height: 100vh;
    }
.form-control {
  background-color: transparent;
  border: 1px solid #fff;
  color: #fff; 
}

.container {
  margin-top: 100px;
  color: #fff;
    }

  </style>
</head>
<body>

<div class="container mt-5">
  <form>

    <div class="form-group">
      <label for="fname">First Name:</label>
      <input type="text" class="form-control" id="fname" required>
    </div>

    <div class="form-group">
      <label for="lname">Last Name:</label>
      <input type="text" class="form-control" id="lname" required>
    </div>

    <div class="form-group">
      <label for="email">Email:</label>
      <input type="email" class="form-control" id="email" required>
    </div>

    <div class="form-group">
      <label for="number">Phone Number:</label>
      <input type="number" class="form-control" id="Number" required>
    </div>

    <div class="form-group">
      <label for="feedback">Feedback:</label>
      <textarea class="form-control" id="feedback" rows="4" required></textarea>
    </div>

    <div class="form-group">
      <label for="rating">Rating:</label>
      <div class="form-check">
        <input class="form-check-input" type="radio" name="rating" id="rating1" value="5" required>
        <label class="form-check-label" for="rating1">
          5 Stars
        </label>
      </div>
      <div class="form-check">
        <input class="form-check-input" type="radio" name="rating" id="rating2" value="4" required>
        <label class="form-check-label" for="rating2">
          4 Stars
        </label>
      </div>
      <div class="form-check">
        <input class="form-check-input" type="radio" name="rating" id="rating3" value="3" required>
        <label class="form-check-label" for="rating3">
          3 Stars
        </label>
      </div>
      <div class="form-check">
        <input class="form-check-input" type="radio" name="rating" id="rating4" value="2" required>
        <label class="form-check-label" for="rating4">
          2 Stars
        </label>
      </div>
      <div class="form-check">
        <input class="form-check-input" type="radio" name="rating" id="rating5" value="1" required>
        <label class="form-check-label" for="rating5">
          1 Star
        </label>
      </div>
    </div>

    <button type="submit" class="btn btn-primary">Submit Feedback</button>
  </form>
</div>

<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

</body>
</html>
```
# Output :
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-10-BOOTSTRAP/assets/80164014/27fb85d0-9fc9-4673-a10f-cc95fe20ee47)

# Objective 2 :
To Create a Responsive student registration form for ABC Engineering College built with Bootstrap.

# Procedure :
## Step 1:
Define Form Fields:

Identify fields required for student registration such as name, email, and course selection.
## Step 2:
Use Bootstrap Components:

Utilize Bootstrap form components for a responsive and visually consistent layout.
## Step 3:
Apply Validation:

Implement HTML5 validation attributes for required fields and email format.
## Step 4:
Enhance User Experience:

Improve user experience by using Bootstrap components like dropdowns for course selection.
## Step 5:
Customize Styling:

Customize the form's appearance to align with ABC Engineering College's branding using Bootstrap and custom CSS.
## Step 6:
Test Across Browsers:

Test the form on different browsers to ensure compatibility.

# Program :
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Student Registration Form</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">

  <style>
    body {
  background: linear-gradient(to right, #6A82FB, #FC5C7D);

.form-control {
  background-color: transparent;
  border: 1px solid #fff;
  color: #fff; 
}

.container {
  margin-top: 100px;
  color: #fff;
}

}
  </style>
</head>
<body>

<div class="container mt-5">
    <form>
      <div class="form-group">
        <label for="studentName">Student Name:</label>
        <input type="text" class="form-control" id="studentName" required>
      </div>
      <div class="form-group">
        <label for="studentEmail">Email:</label>
        <input type="email" class="form-control" id="studentEmail" required>
      </div>
      <div class="form-group">
        <label for="course">Course:</label>
        <select class="form-control" id="course" required>
          <option value="" selected disabled>Select a Course</option>
          <option value="computerScience">Computer Science</option>
          <option value="electricalEngineering">Electrical Engineering</option>
          <option value="mechanicalEngineering">Mechanical Engineering</option>
        </select>
      </div>
      <div class="form-group">
        <label for="dob">Date of Birth:</label>
        <input type="date" class="form-control" id="dob" required>
      </div>
      <div class="form-check">
        <input type="checkbox" class="form-check-input" id="subscribe" />
        <label class="form-check-label" for="subscribe">Subscribe to Newsletter</label>
      </div>

      <button type="submit" class="btn btn-primary">Register</button>
    </form>
  </div>

<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

</body>
</html>
```
# Output :
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-10-BOOTSTRAP/assets/80164014/49a62302-66be-480b-b4fb-7ea723194156)

# Objective 3 :
To Develop a program to structure vertical form layouts which handle form validation in bootstrap.

# Procedure :
## Step 1 :
Create HTML Structure:

Design the HTML structure with Bootstrap's form classes for vertical form layout.
## Step 2 :
Leverage Bootstrap Classes:

Use Bootstrap classes (form, form-group, form-control) to create a vertical form layout.
## Step 3 :
Implement Validation Logic:

Write JavaScript code for basic client-side validation, ensuring required fields are filled.
## Step 4:
Add Error Handling:

Provide feedback to users about validation errors using Bootstrap styles.
## Step 5:
Test Across Browsers:

Test the form and validation logic across different browsers.
## Step 6 :
Optimize for Accessibility:

Ensure the form is accessible, adhering to best practices for users with disabilities.

# Program :
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vertical Form</title>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>
<style>
    footer {
  text-align: center;
  margin-top: 140px;
  padding: 10px;
  background-color: rgba(255, 255, 255, 0.1);
  color: #fff;
}

</style>
<body>

<div class="container mt-5">
    <form id="myForm">
      <div class="form-group">
        <label for="username">Username:</label>
        <input type="text" class="form-control" id="username" required>
      </div>
      <div class="form-group">
        <label for="password">Password:</label>
        <input type="password" class="form-control" id="password" required>
      </div>
      <div class="form-group">
        <label for="confirmPassword">Confirm Password:</label>
        <input type="password" class="form-control" id="confirmPassword" required>
        <small id="passwordError" class="text-danger"></small>
      </div>
  
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
  </div>

  <footer>
    Developed By : Santhan Kumar
  </footer>
  
  <script>
  document.getElementById('myForm').addEventListener('submit', function(event) {
    var password = document.getElementById('password').value;
    var confirmPassword = document.getElementById('confirmPassword').value;
    var passwordError = document.getElementById('passwordError');

    if (password !== confirmPassword) {
      passwordError.textContent = 'Passwords do not match';
      event.preventDefault();
    } else {
      passwordError.textContent = '';
    }
  });
  </script>

<script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.1/dist/umd/popper.min.js"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>

</body>
</html>
```

# Output :
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-10-BOOTSTRAP/assets/80164014/e6975350-3053-4bf0-9350-d49b78a040a7)

# Objective 4 :
To Create a basic email login form in Bootstrap with validation function.

# Procedure :
## Step 1 :
Design Form Elements:

Identify elements needed for an email login form: email input, password input, and submit button.
## Step 2 :
Use Bootstrap Components:

Implement Bootstrap classes (form-group, form-control, btn) for a clean form layout.
## Step 3 :
Incorporate Validation:

Add HTML5 validation attributes and JavaScript code for client-side validation.
## Step 4 :
Apply Styling:

Apply Bootstrap styling for a consistent and visually appealing design.
## Step 5 :
Test Responsiveness:

Ensure the form is responsive by testing it on various devices.
## Step 6 :
Test Login Functionality:

Validate the login form by testing the login functionality on the server side.

# Program :
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Validation</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(to right, #3498db, #1abc9c);
            color: #fff;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
        }

        h2 {
            color: #fff;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            margin-bottom: 30px;
        }

        form {
            width: 80%;
            max-width: 400px;
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
        }

        label {
            display: block;
            margin-bottom: 8px;
            color: #333;
        }

        input {
            width: calc(100% - 16px);
            padding: 12px;
            margin-bottom: 16px;
            border: 2px solid #3498db;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 16px;
            color: #333;
        }

        button {
            background-color: #4CAF50;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover {
            background-color: #45a049;
        }

        .error-message {
            color: red;
            margin-top: -8px;
            margin-bottom: 16px;
            text-align: left;
        }

        footer {
  text-align: center;
  margin-top: 70px;
  padding: 10px;
  background-color: rgba(255, 255, 255, 0.1);
  color: #fff;
}
    </style>
</head>
<body>

    <h2>Form Validation</h2>

    <footer>
        Developed By : Santhan Kumar
    </footer>

    <form id="myForm" onsubmit="validateForm(); return false;">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name">
        <div id="nameError" class="error-message"></div>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email">
        <div id="emailError" class="error-message"></div>

        <button type="submit">Submit</button>
    </form>

    <script>
        function validateForm() {
            document.getElementById('nameError').innerText = '';
            document.getElementById('emailError').innerText = '';

            var name = document.getElementById('name').value;
            var email = document.getElementById('email').value;

            if (name.trim() === '') {
                document.getElementById('nameError').innerText = 'Name is required.';
            }

            if (email.trim() === '') {
                document.getElementById('emailError').innerText = 'Email is required.';
            } else if (!isValidEmail(email)) {
                document.getElementById('emailError').innerText = 'Invalid email format.';
            }
        }

        function isValidEmail(email) {
            var emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return emailRegex.test(email);
        }
    </script>

</body>
</html>
```

# Output :
![image](https://github.com/SANTHAN-2006/ODD2023-WT-Ex-10-BOOTSTRAP/assets/80164014/b331ac5d-0bc0-41e6-b8d5-870d68d92dc2)

# Result :
Successfully executed all the given programs using bootstrap.
## Name : guntur shaik mohammad shahil
## Register Number : 212223240044
