# week-2-web-dev
web development week 2 assignment

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Enhanced Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 40px;
      background: #f4f4f4;
    }
    h1 {
      color: #333;
    }
    form {
      background: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    label {
      display: block;
      margin: 15px 0 5px 0;
      font-weight: bold;
    }
    input, select, textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    button {
      background: #007BFF;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 4px;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
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
      background: #f2f2f2;
    }
    img {
      max-width: 100%;
      height: auto;
    }
  </style>
</head>
<body>

  <h1>Enhanced Form</h1>

  <form action="/submit" method="post">
    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name" placeholder="Enter your full name" required autocomplete="name" />

    <label for="email">Email Address:</label>
    <input type="email" id="email" name="email" placeholder="you@example.com" required autocomplete="email" />

    <label for="age">Age:</label>
    <input type="number" id="age" name="age" min="1" max="120" placeholder="Enter your age" required />

    <label for="gender">Gender:</label>
    <select id="gender" name="gender" required>
      <option value="">Select gender</option>
      <option value="male">Male</option>
      <option value="female">Female</option>
      <option value="other">Other</option>
    </select>

    <label for="hobbies">Hobbies:</label>
    <input type="text" id="hobbies" name="hobbies" placeholder="Enter your hobbies (comma-separated)" autocomplete="off" />

    <label for="bio">Bio:</label>
    <textarea id="bio" name="bio" rows="4" placeholder="Write a short bio about yourself"></textarea>

    <label for="profile-pic">Profile Picture (URL):</label>
    <input type="url" id="profile-pic" name="profile-pic" placeholder="Enter image URL" readonly />

    <label for="contact">Contact Information:</label>
    <table>
      <tr>
        <th>Phone</th>
        <th>Address</th>
      </tr>
      <tr>
        <td><input type="tel" id="phone" name="phone" placeholder="Phone number" required /></td>
        <td><input type="text" id="address" name="address" placeholder="Street address" required /></td>
      </tr>
    </table>

    <button type="submit">Submit</button>
  </form>

</body>
</html>
