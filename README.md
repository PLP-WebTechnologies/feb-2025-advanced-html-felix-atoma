# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨
the answers
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ghana Connect</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        .container {
            width: 90%;
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
        }
        h1, h2 {
            text-align: center;
            color: #2c3e50;
        }
        ol {
            list-style-type: upper-roman;
            padding-left: 20px;
        }
        .image-container {
            text-align: center;
            margin: 20px 0;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 10px;
            text-align: left;
        }
        th {
            background-color: #4CAF50;
            color: white;
        }
        form {
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            margin-top: 20px;
        }
        input, select, button {
            width: 100%;
            padding: 10px;
            margin: 8px 0;
            display: block;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background-color: #F7931E;
            color: white;
            font-weight: bold;
            cursor: pointer;
            border: none;
        }
        button:hover {
            background-color: #D17B15;
        }
        .form-group {
            margin-bottom: 15px;
        }
        .form-group label {
            font-weight: bold;
        }
        .checkbox-group {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        /* Responsive Design */
        @media (max-width: 600px) {
            .container {
                padding: 10px;
            }
            table, th, td {
                font-size: 14px;
            }
        }
    </style>
</head>
<body>

    <!-- Ordered List -->
    <div class="container">
        <h2>Traditional Ghanaian Dishes</h2>
        <ol type="I">
            <li>Waakye</li>
            <li>Jollof Rice</li>
            <li>Banku and Tilapia</li>
            <li>Fufu with Light Soup</li>
            <li>Kelewele</li>
        </ol>
    </div>

    <!-- Ghanaian Image -->
    <div class="image-container">
        <img src="https://upload.wikimedia.org/wikipedia/commons/7/71/Independence_Arch_Accra.jpg" alt="Independence Arch, Accra">
    </div>

    <!-- Table -->
    <div class="container">
        <h2>Contact List</h2>
        <table border="1">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>City</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Kofi Mensah</td>
                    <td>Accra</td>
                    <td>+233 24 123 4567</td>
                    <td>kofi.mensah@example.com</td>
                </tr>
                <tr>
                    <td>Afia Owusu</td>
                    <td>Kumasi</td>
                    <td>+233 26 987 6543</td>
                    <td>afia.owusu@email.com</td>
                </tr>
                <tr>
                    <td>Yaw Boateng</td>
                    <td>Tamale</td>
                    <td>+233 50 678 9123</td>
                    <td>yaw.boateng@example.com</td>
                </tr>
                <tr>
                    <td>Akua Djan</td>
                    <td>Cape Coast</td>
                    <td>+233 55 789 4321</td>
                    <td>akua.djan@email.com</td>
                </tr>
            </tbody>
        </table>
    </div>

    <!-- Registration Form -->
    <div class="container">
        <h2>Registration Form</h2>
        <form>
            <div class="form-group">
                <label for="name">Full Name</label>
                <input type="text" id="name" placeholder="Enter your full name" required>
            </div>
            <div class="form-group">
                <label for="email">Email Address</label>
                <input type="email" id="email" placeholder="Enter your email" required>
            </div>
            <div class="form-group">
                <label for="password">Password</label>
                <input type="password" id="password" placeholder="Enter password" required>
            </div>
            <div class="form-group">
                <label for="dob">Date of Birth</label>
                <input type="date" id="dob" required>
            </div>
            <div class="form-group">
                <label>Gender</label>
                <div class="checkbox-group">
                    <label><input type="radio" name="gender" value="male"> Male</label>
                    <label><input type="radio" name="gender" value="female"> Female</label>
                    <label><input type="radio" name="gender" value="other"> Other</label>
                </div>
            </div>
            <div class="form-group">
                <label for="role">Role</label>
                <select id="role" required>
                    <option value="">Select your role</option>
                    <option value="farmer">Farmer</option>
                    <option value="distributor">Distributor</option>
                    <option value="consumer">Consumer</option>
                </select>
            </div>
            <div class="form-group">
                <label>Interests</label>
                <div class="checkbox-group">
                    <label><input type="checkbox" name="interests" value="farming"> Sustainable Farming</label>
                    <label><input type="checkbox" name="interest" value="environment"> Environmental Sustainability</label>
                    <label><input type="checkbox" name="business" value="entrepreneurship"> Entrepreneurship</label>
                </div>
            </div>
            <button type="submit">Register</button>
        </form>
    </div>

</body>
</html>

