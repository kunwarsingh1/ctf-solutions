According to the natas8 webpage we have to use the username natas8 and the password from the previous challenge that we found.


When accessing the source code we come accross a hash function which can be reversed i.e.  bin2hex(strrev(base64_encode($secret))) and the secret is also
given so using online php compiler we decrypt the has by using the script---

$encoded = "your_encoded_string_here"; // Replace with the actual encoded string
$step1 = hex2bin($encoded); // Reverse bin2hex
$step2 = strrev($step1);    // Reverse strrev
$step3 = base64_decode($step2); // Reverse base64_encode
echo $step3; // This will output the original $secret


and use that as an input to the main page and we get the password----


Access granted. The password for natas9 is <password> 
