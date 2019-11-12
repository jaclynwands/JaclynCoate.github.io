# JaclynCoate.github.io
Website to display my personal projects and anlyses. Enjoy!

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {font-family: Arial;}

/* Style the tab */
.tab {
  overflow: hidden;
  border: 1px solid #ccc;
  background-color: #f1f1f1;
}

/* Style the buttons inside the tab */
.tab button {
  background-color: inherit;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  transition: 0.3s;
  font-size: 17px;
}

/* Change background color of buttons on hover */
.tab button:hover {
  background-color: #ddd;
}

/* Create an active/current tablink class */
.tab button.active {
  background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
  display: none;
  padding: 6px 12px;
  border: 1px solid #ccc;
  border-top: none;
}
</style>
</head>
<body>

<h2>Tabs</h2>
<p>Click on the buttons inside the tabbed menu:</p>

<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'About Me')">About Me</button>
  <button class="tablinks" onclick="openCity(event, 'DS 6306: Case Study 1')">DS 6306: Case Study 1</button>
  <button class="tablinks" onclick="openCity(event, 'DS 63036: Final Project')">DS 63036: Final Project</button>
</div>

<div id="About Me" class="tabcontent">
  <h3>About Me</h3>
  <p>About Me Information.</p>
</div>

<div id="DS 6306: Case Study 1" class="tabcontent">
  <h3>DS 6306: Case Study 1</h3>
  <p>DS 6306: Case Study 1 work</p> 
</div>

<div id="DS 63036: Final Project" class="tabcontent">
  <h3>DS 63036: Final Project</h3>
  <p>DS 63036: Final Project</p>
</div>

<script>
function openCity(evt, cityName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>
   
</body>
</html>
