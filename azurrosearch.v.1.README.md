<?php
include_once 'azurroheader.php';
?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AzurroCheck</title>
</head>
<body>
                <div class="main">
                        <div class="text">
                           <h3>Private site for Azurro Garden owners.</h>
                           <h3>...........................................</h>
             
                        </div>

                        <form action="azurrosearchdb.php" method="POST">

                                  <label for="entersearch">Pleace, enter :</label><br>
                                  <input type="text" id="entersearch" name="entersearch" placeholder="Enter apartment you want to search ..."><br>

                                  <input type="submit" id="submitbuton" value="Submit"><br><br>
                        </form>
                        
                </div>  
    
</body>
</html>
<?php
include_once 'azurrofooter.php';
?>
