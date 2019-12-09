
<html>

<head>
<meta http-equiv="Content-Type" content="text/html; charset=tis-620">
<title>ทำการสุ่ม Random ตัวเลข ทั้งแบบ ไม่ซ้ำ และ ซ้ำ ด้วย PHP</title>
<STYLE type=text/css>
  A:link { color: #0000cc; text-decoration:none}
  A:visited {color: #0000cc; text-decoration: none}
  A:hover {color: red; text-decoration: none}
 </STYLE>
<style type="text/css">
<!--
small { font-family: Arial, Helvetica, sans-serif; font-size: 8pt; } 
input, textarea { font-family: Arial, Helvetica, sans-serif; font-size: 9pt; } 
b { font-family: Arial, Helvetica, sans-serif; font-size: 12pt; } 
big { font-family: Arial, Helvetica, sans-serif; font-size: 16pt; } 
strong { font-family: Arial, Helvetica, sans-serif; font-size: 11pt; font-weight : extra-bold; } 
font, td { font-family: Arial, Helvetica, sans-serif; font-size: 11pt; } 
BODY { font-size: 11pt; font-family: Arial, Helvetica, sans-serif; } 
-->
</style>

</head>
<!DOCTYPE html>
<html>
<body>
<center><u><big>ทำการสุ่ม Random ตัวเลข ทั้งแบบ ไม่ซ้ำ และ ซ้ำ ด้วย PHP</big></u></center>

<br><br>
<u>สุ่มตัวเลข 1-10 แบบไม่ซ้ำ</u>

<br><br>&nbsp;&nbsp;&nbsp;&nbsp;หลักการคือ จะทำการสุ่มตัวเลขลงใน Array โดยจะไม่มีการสุ่มตัวเลขซ้ำกัน ตัวไหนโดนสุ่มไปแล้ว จะไม่สุ่มออกมาอีก โดยค่าที่ถูกสุ่มจะไปเก็บไว้ใน Array


<br><br>
<?php

$arr_random_number = range(1,10); // คือกำหนดช่วงของตัวเลขที่ต้องการให้สุ่มออกมาก่อน

shuffle($arr_random_number); // เป็นคำสั่งสลับแต่ละแหน่งของข้อมูลใน Array แบบ Random

$arr_index = 0;

foreach ($arr_random_number as $text_tmp)
{
     echo "\$arr_random_number[$arr_index] = ".$text_tmp."<br>"; 
     $arr_index++;
}

?>

<br>
<u>สุ่มตัวเลข 1-10 แบบซ้ำ</u>

<br><br>&nbsp;&nbsp;&nbsp;&nbsp;ใช้คำสั่ง Random พื้นๆ ของ PHP ไม่ต้องประยุกต์อะไร

<br><br>

<?

$no = 1;

for($i=0;$i<10;$i++)
{
     echo "สุ่มครั้งที่ $no = ".rand (1,10)."<br>"; 
     $no++;
}

?>

<br><br>
<hr width="75%">
<center><big>สนับสนุนโดย : <a href="http://www.codetukyang.com" target="_blank">CodeTukYang.Com</a></big></center>
<hr width="75%">
</body>

</html>

<h2>My First JavaScript</h2>

<button type="button"
onclick="document.getElementById('demo').innerHTML = Date()">
Click me to display Date and Time.</button>

<p id="demo"></p>

</body>
</html> 

