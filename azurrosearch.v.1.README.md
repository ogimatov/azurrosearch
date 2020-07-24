<?php
include_once 'azurroheader.php';
?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" type="text/css" href="azurrostyle.css" media="screen"/>
    <title>AzurroSearch</title>
</head>
<body>
                    <div class="main">
                            <div class="text">
                            <h3>Private site for Azurro Garden owners.</h>
                            <h3>...........................................</h>            
                            </div>

                                <div class = "search">
                                    <?php
                                            $servername='localhost';
                                            $username='root';
                                            $password='ogi123456';
                                            $dbname = "azurrodb";
                                    
                                            $link = mysqli_connect("localhost", "root", "ogi123456", "azurrodb");

                                            if($link === false)
                                            {
                                            die("ERROR: Could not connect. " . mysqli_connect_error());
                                            }
                                            // $fev = 'Гари';
                                            // echo $fev;
                                            // $fstchar = 'Г';
                                            // echo $fstchar;

                                            $search = "SELECT * FROM azurroinfo WHERE apartnumber LIKE 'fstchar%'";

                                                if($result = mysqli_query($link, $search))
                                                        {
                                                            while($rows = mysqli_fetch_assoc($result))
                                                            {
                                                                foreach($rows as $key => $val)
                                                                {
                                                                    echo $val;
                                                                    
                                                                }
                                                            }
                                                        }

                                    ?>
                                </div>
                    </div>
    
</body>
</html>
<?php
include_once 'azurrofooter.php';
?>
