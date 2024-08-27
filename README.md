<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Registration Form Using Table</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to bottom, #99ccff, #cc99ff);
            margin: 0;
            padding: 20px;
        }

        table {
            border: 2px dashed black;
            padding: 20px;
            background-color: white;
            margin: 0 auto;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        th {
            font-size: 24px;
            text-align: center;
            padding-bottom: 10px;
        }

        td {
            padding: 10px;
            vertical-align: top;
        }

        input[type="text"], input[type="email"], input[type="number"], select, textarea {
            width: 100%;
            padding: 8px;
            box-sizing: border-box;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        input[type="radio"], input[type="checkbox"] {
            margin-right: 10px;
        }

        input[type="submit"], input[type="reset"] {
            width: 100px;
            padding: 8px;
            margin: 10px 5px;
            border: none;
            background-color: #4CAF50;
            color: white;
            border-radius: 4px;
            cursor: pointer;
        }

        input[type="submit"]:hover, input[type="reset"]:hover {
            background-color: #45a049;
        }

        h2 {
            text-align: center;
            font-family: Arial, sans-serif;
            font-size: 22px;
        }
    </style>
</head>
<body>
    <h2>Student Registration Form Using Table in HTML</h2>
    <form>
        <table>
            <tr>
                <th colspan="2">Student Registration Form</th>
            </tr>
            <tr>
                <td>First Name:</td>
                <td><input type="text" name="first_name" maxlength="50"></td>
            </tr>
            <tr>
                <td>Last Name:</td>
                <td><input type="text" name="last_name" maxlength="50"></td>
            </tr>
            <tr>
                <td>Email ID:</td>
                <td><input type="email" name="email"></td>
            </tr>
            <tr>
                <td>Mobile Number:</td>
                <td><input type="text" name="mobile" maxlength="10"></td>
            </tr>
            <tr>
                <td>Gender:</td>
                <td>
                    <input type="radio" name="gender" value="male"> Male
                    <input type="radio" name="gender" value="female"> Female
                </td>
            </tr>
            <tr>
                <td>Date of Birth (DOB):</td>
                <td>
                    <select name="day">
                        <option>Day</option>
                        <!-- Add days here -->
                    </select>
                    <select name="month">
                        <option>Month</option>
                        <!-- Add months here -->
                    </select>
                    <select name="year">
                        <option>Year</option>
                        <!-- Add years here -->
                    </select>
                </td>
            </tr>
            <tr>
                <td>Address:</td>
                <td><textarea name="address" rows="4" cols="50"></textarea></td>
            </tr>
            <tr>
                <td>City:</td>
                <td><input type="text" name="city" maxlength="50"></td>
            </tr>
            <tr>
                <td>Pin Code:</td>
                <td><input type="text" name="pin_code" maxlength="6"></td>
            </tr>
            <tr>
                <td>State:</td>
                <td><input type="text" name="state" maxlength="50"></td>
            </tr>
            <tr>
                <td>Country:</td>
                <td><input type="text" name="country" value="India" readonly></td>
            </tr>
            <tr>
                <td>Hobbies:</td>
                <td>
                    <input type="checkbox" name="hobbies" value="drawing"> Drawing
                    <input type="checkbox" name="hobbies" value="singing"> Singing
                    <input type="checkbox" name="hobbies" value="dancing"> Dancing
                    <input type="checkbox" name="hobbies" value="sketching"> Sketching
                    <input type="checkbox" name="hobbies" value="others"> Others: <input type="text" name="other_hobbies" maxlength="50">
                </td>
            </tr>
            <tr>
                <td>Qualification:</td>
                <td>
                    <input type="checkbox" name="qualification" value="high_school"> High School(10th)<br>
                    <input type="checkbox" name="qualification" value="higher_school"> Higher School(12th)<br>
                    <input type="checkbox" name="qualification" value="graduation"> Graduation(Bachelors)<br>
                    <input type="checkbox" name="qualification" value="post_graduation"> Post Graduation(Masters)<br>
                    <input type="checkbox" name="qualification" value="phd"> Phd
                </td>
            </tr>
            <tr>
                <td>Courses Applied For:</td>
                <td>
                    <input type="radio" name="course" value="bca"> BCA(Bachelor of Computer Applications)<br>
                    <input type="radio" name="course" value="bcom"> B.Com(Bachelor of Commerce)<br>
                    <input type="radio" name="course" value="bsc"> B.Sc(Bachelor of Science)<br>
                    <input type="radio" name="course" value="ba"> BA(Bachelor of Arts)<br>
                    <input type="radio" name="course" value="mca"> MCA(Master of Computer Applications)<br>
                    <input type="radio" name="course" value="mcom"> M.Com(Master of Commerce)<br>
                    <input type="radio" name="course" value="msc"> M.Sc(Master of Science)<br>
                    <input type="radio" name="course" value="ma"> MA(Master of Arts)
                </td>
            </tr>
            <tr>
                <td colspan="2" style="text-align: center;">
                    <input type="submit" value="Submit">
                    <input type="reset" value="Reset">
                </td>
            </tr>
        </table>
    </form>
</body>
</html>