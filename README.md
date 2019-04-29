<html>

<body>

<style>

  

::-webkit-datetime-edit { padding: 1em; }

::-webkit-datetime-edit-fields-wrapper { background: silver; }

::-webkit-datetime-edit-text { color: red; padding: 0 0.3em; }

::-webkit-datetime-edit-month-field { color: blue; }

::-webkit-datetime-edit-day-field { color: green; }

::-webkit-datetime-edit-year-field { color: purple; }

::-webkit-inner-spin-button { display: none; }

::-webkit-calendar-picker-indicator { background: orange; }



.label {

  color: white;

  padding: 8px;

}



.success {background-color: #4CAF50;} /* Green */

.info {background-color: #2196F3;} /* Blue */

.warning {background-color: #ff9800;} /* Orange */

.danger {background-color: #f44336;} /* Red */ 

.other {background-color: #e7e7e7; color: black;} /* Gray */



.button {

  background-color: #4CAF50; /* Green */

  border: none;

  color: white;

  padding: 15px 32px;

  text-align: center;

  text-decoration: none;

  display: inline-block;

  font-size: 16px;

}

</style>

<script

  src="https://code.jquery.com/jquery-3.4.0.js"

  crossorigin="anonymous"></script>



  <script type="text/javascript">



function getDay()

{

var weekday = ["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"];



var a = new Date($("#dateId").val());

//alert(a);

//alert(weekday[a.getDay()]);

$("#result").empty();

if(weekday[a.getDay()]  = 'undefined')

$("#result").append($("<p> <span class='label danger'>  INVALID   DATE  </span>  </p>"));

else

$("#result").append($("<p> <span class='label success'>  The Day Is : " + weekday[a.getDay()] + "   </span>  </p>"));





 

}



</script>

<div id="dateDiv">

<span class=" "> Enter Date :  </span>

<input  type="Date" id="dateId" />



<input type="button" value="get The Day" id="button" class="button"  onclick="getDay()" />



</div>

<div id="result" >



</div>

</body>

</html>
