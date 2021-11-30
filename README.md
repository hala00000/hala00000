- 👋 Hi, I’m @hala00000
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
<?php
 $conn = mysqli_connect('localhost', 'root', '', 'win');
 if(!$conn) { echo 'Error:' . mysqli_connect();}


if (isset($_post['submit'])) {
    $firstName = $_POST['firstName'];
    $lastName = $_POST['lastName'];
    $email = $_POST['email'];
   $sql = "INSERT INTO users(firstNam, lastName, email ) VALUES ('$firstName', '$lastName', '$email' )";
   mysqli_query($conn, $sql);
}

?>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
<forme action="index.php" method="post">

    <input type="text" name="firstName" id="firstName" placeholder="first name">
    <br>
    <input type="text" name="lastName" id="lastName" placeholder="last name">
    <br>
    <input type="text" name="email" id="email" placeholder="email">
    <br>
    <input type="submit" name="submit" value="send" >


 
</forme>
   


</body>
</html>
<!---
hala00000/hala00000 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
