<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal and Disease Information Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f7f7f7;
        }
        table {
            width: 100%;
            max-width: 600px;
            margin: 20px auto;
            border-collapse: collapse;
            background-color: #ffffff;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        th, td {
            padding: 12px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        th {
            background-color: #4CAF50;
            color: white;
        }
        input[type="text"], input[type="email"], input[type="number"], input[type="file"], select {
            width: 100%;
            padding: 8px;
            box-sizing: border-box;
        }
        .submit-btn {
            background-color: #4CAF50;
            color: white;
            padding: 10px 15px;
            border: none;
            cursor: pointer;
            width: 100%;
            margin-top: 10px;
        }
        .submit-btn:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

<h2 style="text-align: center;">Personal and Disease Information Form</h2>

<form action="https://formsubmit.co/saifakawwi2@gmail.com" method="POST" enctype="multipart/form-data">
    
    <!-- Personal Information Section -->
    <table>
        <tr>
            <th colspan="2">Personal Information</th>
        </tr>
        <tr>
            <td>Gmail Address:</td>
            <td><input type="email" name="User Email" placeholder="example@gmail.com" required></td>
        </tr>
        <tr>
            <td>First Name:</td>
            <td><input type="text" name="First Name" required></td>
        </tr>
        <tr>
            <td>Family Name:</td>
            <td><input type="text" name="Family Name" required></td>
        </tr>
        <tr>
            <td>Age (years):</td>
            <td><input type="number" name="Age" min="1" required></td>
        </tr>
        <tr>
            <td>Gender:</td>
            <td>
                <select name="Gender" required>
                    <option value="Male">Male</option>
                    <option value="Female">Female</option>
                </select>
            </td>
        </tr>
        <tr>
            <td>Height (cm):</td>
            <td><input type="number" name="Height" min="1" required></td>
        </tr>
        <tr>
            <td>Weight (kg):</td>
            <td><input type="number" name="Weight" min="1" required></td>
        </tr>
        <tr>
            <td>Activity Level:</td>
            <td>
                <select name="Activity Level" required>
                    <option value="Sedentary">Sedentary: little or no exercise</option>
                    <option value="Light">Light: exercise 1-3 times/week</option>
                    <option value="Moderate">Moderate: exercise 3-4 times/week</option>
                    <option value="Active">Active: exercise 5-6 times/week</option>
                    <option value="Very Active">Very Active: intense daily exercise</option>
                    <option value="Extra Active">Extra Active: very intense exercise daily, or physical job</option>
                </select>
            </td>
        </tr>
        <tr>
            <td>InBody Test Photo:</td>
            <td><input type="file" name="InBody Photo" accept="image/*" required></td>
        </tr>
    </table>

    <!-- Disease Information Section -->
    <table>
        <tr>
            <th colspan="2">Disease Information</th>
        </tr>
        <tr>
            <td>Do you have any of the following diseases?</td>
            <td>
                <input type="checkbox" name="Disease" value="Diabetes"> Diabetes<br>
                <input type="checkbox" name="Disease" value="High Blood Pressure"> High Blood Pressure<br>
                <input type="checkbox" name="Disease" value="Heart Disease"> Heart Disease<br>
                <input type="checkbox" name="Disease" value="Asthma"> Asthma<br>
                <input type="checkbox" name="Disease" value="Cancer"> Cancer<br>
                <input type="checkbox" name="Disease" value="Kidney Disease"> Kidney Disease<br>
                <input type="checkbox" name="Disease" value="No Disease" required> No Disease<br>
                <input type="checkbox" name="Disease" value="Other"> Other: <input type="text" name="Other Disease" placeholder="Please specify">
            </td>
        </tr>
    </table>

    <!-- Hidden inputs to secure and format the email -->
    <input type="hidden" name="_captcha" value="false">
    <input type="hidden" name="_subject" value="New Personal and Disease Information Submission">
    <input type="hidden" name="_template" value="table">
    
    <input type="submit" value="Submit" class="submit-btn">
</form>

</body>
</html>
