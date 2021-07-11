<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">	
<link rel="shortcut icon" href="http://imgur.com/CILKGax.png" >
<title>Phạm Ngọc Phú</title> <!-- BẠN THAY ĐỔI TIÊU ĐỀ Ở ĐÂY-->
<link rel="stylesheet" href="css3/popup.css">
<link rel="stylesheet" href="css3/styles.css">
<link href='http://fonts.googleapis.com/css?family=Source+Sans+Pro&subset=latin,vietnamese' rel='stylesheet' type='text/css'>
<script type="text/javascript" src="http://code.jquery.com/jquery-1.6.min.js"></script>
<script type="text/javascript" src="jss/jquery.popup.js"></script>
<script src="jss/popup.js" type="text/javascript"></script>
<script src="jss/jquery-1.js" type="text/javascript"></script>
<script type="text/javascript" src="jss/jquery.js"></script>

<script type="text/javascript">

$(document).ready(function () {

	// if user clicked on button, the overlay layer or the dialogbox, close the dialog	
	$('a.btn-ok, #msb-nt').click(function () {		
		$('#dialog-overlay, #dialog-box').hide();		
		return false;
	});
	
	// if user resize the window, call the same function again
	// to make sure the overlay fills the screen and dialogbox aligned to center	
	$(window).resize(function () {
		

		if (!$('#dialog-box').is(':hidden')) popup();		
	});	
	
	
