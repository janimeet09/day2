# day2
<?php
	error_reporting(0);
	if(isset($_POST["ans"]))
	{
		$no1= $_POST["no1"];
		
		if($no1 %2==0)
		{
			$ans= "number is Even";
		}
		else
		{
			$ans= "Number is odd";		
		}
	}
?>
<html>
<head>
<title>Task__1</title>
</head>
<body>
<form action="" method="post">
<table border="2" align="center">
<tr>
	<td> Enter value :- </td>
	<td><input type="text" name="no1"></td>
</tr>	

<tr>
		<td><input type="submit" name="ans" value="submit"></td>
</tr>
<tr>
	<td>Answee is :- </td>
	<td><input type="text" name="no2" value="<?php echo $ans; ?>"></td>
</table>
</form>
</body>
</html>
