# Oasis-infobyte-task1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gyaan Peet - School Registration</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px;
            text-align: center;
        }
        h1 {
            margin: 0;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            padding: 20px;
            background-color: white;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin: 10px 0 5px;
            font-weight: bold;
        }
        input[type="text"],
        input[type="email"],
        input[type="tel"],
        input[type="date"],
        textarea,
        select {
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }
        textarea {
            resize: vertical;
        }
        input[type="submit"] {
            background-color: #4CAF50;
            color: white;
            padding: 15px;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

    <header>
        <h1>Welcome to Gyaan Peet</h1>
        <p>Your Gateway to Quality Education</p>
    </header>

    <div class="container">
        <h2>Student Enrollment Form</h2>
        <form action="/submit_registration" method="POST">
            <label for="student_name">Student Name:</label>
            <input type="text" id="student_name" name="student_name" required>

            <label for="dob">Date of Birth:</label>
            <input type="date" id="dob" name="dob" required>

            <label for="parent_name">Parent/Guardian Name:</label>
            <input type="text" id="parent_name" name="parent_name" required>

            <label for="contact">Contact Number:</label>
            <input type="tel" id="contact" name="contact" required>

            <label for="email">Email Address:</label>
            <input type="email" id="email" name="email" required>

            <label for="address">Address:</label>
            <textarea id="address" name="address" rows="4" required></textarea>

            <label for="class">Class Enrolling For:</label>
            <select id="class" name="class" required>
                <option value="">Select Class</option>
                <option value="Nursery">Nursery</option>
                <option value="LKG">LKG</option>
                <option value="UKG">UKG</option>
                <option value="1">Class 1</option>
                <option value="2">Class 2</option>
                <option value="3">Class 3</option>
                <option value="4">Class 4</option>
                <option value="5">Class 5</option>
                <option value="6">Class 6</option>
                <option value="7">Class 7</option>
                <option value="8">Class 8</option>
                <option value="9">Class 9</option>
                <option value="10">Class 10</option>
            </select>

            <input type="submit" value="Register">
        </form>
    </div>

</body>
</html>
