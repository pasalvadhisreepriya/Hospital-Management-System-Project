<%@ page language="java" contentType="text/html; charset=ISO-8859-1"
	pageEncoding="ISO-8859-1"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title>Home Page</title>
<style type="text/css">
h1 {
	width: 1300px;
	border: 12px solid rgb(0, 179, 173);
	padding: 6px;
	margin: 5px;
	text-align: center;
	border-radius: 5px;
}
a {
	text-decoration: none;
	background-color: rgb(39, 129, 206);
	color: white;
	padding: 5px;
	border-radius: 2px;
}
li {
	float: left;
	padding: 2px;
	margin-left: 170px;
	font-weight: bold;
	font-size: 18px;
}
ul {
	background-color: rgb(0,179,173);
	list-style-type: none;
	overflow: hidden;
	padding: 10px;
	margin: 10px;
}
</style>
</head>
<body>
	<h1>Hospital DBMS</h1>
	<img src="hsptl.jpg" alt="front image" width="1350" height="450">
	<ul>
		<li>Admin Login <a href="AdmLogin.jsp">LOGIN</a></li>
		<li>Doctor Login <a href="DocLogin.jsp">LOGIN</a></li>
		<li>Patient Login <a href="PatLogin.jsp">LOGIN</a></li>
	</ul>
	
	<section class="container border border-dark space">
		<h1>Hospital Management System</h1>
		<p class="text-lg">This is a hospital management user interface
			for managing, monitoring and controlling the system in a hospital.
			This application is developed using java, which mainly focuses on
			basic operations in a hospital like adding new patient information,
			and updating new information, assigning the doctor for patient. It
			features a familiar and well thought-out, an attractive online user
			interface, combined with strong management capabilities. The backend
			of the project is</p>
	</section>
</body>
</html>