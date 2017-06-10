# Reserveringssysteem-t-Fust

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Reserveren - Café 't Fust Rotterdam</title>
    <link rel="stylesheet" type="text/css" href="reservering.css">
    <link rel="icon" href="img/gothic-alphabet-letter-f.jpg">


</head>

<body>

<img src="img/Biercafe-Rotterdam.png" class="logo" width="182" height="158" alt="Café 't Fust">

<div class="patternright1">
    <img src="img/1194989366182291164pattern-dots-square-grid-02.svg.med.png" height="150"/>
</div>

<div class="patternright2">
    <img src="img/1194989366182291164pattern-dots-square-grid-02.svg.med.png" height="150"/>
</div>

<div class="patternleft1">
    <img src="img/1194989366182291164pattern-dots-square-grid-02.svg.med.png" height="150"/>
</div>

<div class="patternleft2">
    <img src="img/1194989366182291164pattern-dots-square-grid-02.svg.med.png" height="150"/>
</div>

<div class="feyenoordlogo">
    <img src="img/1024px-Feyenoord_logo.svg.png" width="75" height="75"/>
</div>


<br>
<br>



<header>
    <div class="container group">

        <h1>  Reserveren </h1>
    </div>
</header>

<h2> Vul uw gewenste gegevens in en wij regelen het voor u!</h2>

<?php
if(isset($_POST['tafelzone'])){
    $zone = $_POST['tafelzone'];
}
?>

<form action="inserted.php" method="post">

    <div>
        <input type="text" id="voornaam" name="voornaam" placeholder="Voornaam*" />
    </div>
    <br>
    <div>
        <input type="text" id="achternaam" name="achternaam" placeholder="Achternaam*" />
    </div>
    <br>
    <div>
        <input type="text" id="aantaltafels" name="aantaltafels" placeholder="Aantal tafels*" />
    </div>
    <br>
    <div>
        <input type="text" id="tafelzone" name="tafelzone" placeholder="Tafelzone(1 t/m 4)*" />
    </div>
    <br>
    <div>

        <input type="text" id="personen" name="personen" placeholder="Aantal personen*" />
    </div>
    <br>
    <div>
        <input type="text" id="telefoonnummer" name="telefoonnummer" placeholder="Telefoonnummer*" />
    </div>
    <br>
    <div>
        <label for="dag"></label><input name="dag" type="date" id="dag" />
    </div>

    <br>
    <div>
        <label for="tijd"></label><input name="tijd" type="time" id="tijd" />
    </div>

    <br>
    <div class="bericht">

        <textarea name="bericht" placeholder="Extra info*"></textarea>
    </div>

    <div class="button">
        <button type="submit" name="submit" value="add">Verzenden</button>
    </div>

    <div class="duvel">
        <img src="img/duvels.png" alt="">
    </div>

    <div class="burger">
        <img src="img/010burger.png" alt="">
    </div>

</form>
</body>
</html>
