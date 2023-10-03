# InternetOfThings

<H1> LEDstrip kleur via een colorpicker in via Adafruit IO </H1> 


Stappen die je doorloopt om succesvol een DIY Philips Lampje te maken doormiddel van het NodeMCU board + een ledstripje:


<H2>Stap 1: </H2>
<ol>
  <li>Instaleer de library Adafruit IO Arduino in de Arduino applicatie. Tools -> Manage labraries</li>
  <li>Zorg er ook voor dat je board de goede board manager heeft en aangesloten is op het goede port, om verbindingsproblemen te voorkomen</li>
  <li>Sluit daarnaast je ledstrip aan op (van ledstrip naar board): +5V -> 3V3 | DIN -> D5 | GND -> GND </li>
</ol>

<H2>Stap 2: </H2>
<ol>
<li> Ga naar https://io.adafruit.com/ en maak een gratis account aan. </li>
<li> Als deze is aangemaakt ga je naar https://io.adafruit.com/overview (Dit was voor mij niet duidelijk, als het niet te vinden is, ga in google en zoek Adafruit overview. Dan kom je op de goede pagina terecht.) </li>
</ol>

<H2>Stap 3: </H2>
<ol>
<li>  Klik op de pagina de gele sleutel aan en kopieer je username en key. </li>
<li>  Maak vervolgens een dashboard aan, onder kopje dashboard en klik 'nieuw dashboard aanmaken.'Geef het een naam en een discriptie. Sla deze vervolgens op. </li>
<li>  Klik op het dashboard en maak een nieuw blok aan. (Dit is het tandwieltje) Kies uit de lijst de colorpicker en maak een nieuwe feed aan die je 'Color' noemt. Sla dit op en selecteer de Color feed en klik op Next Step. Geef het block een leuke optionele titel en creeer het blok. </li>
<li> Klik vervolgens in het dashboard op de color picker om hiervan de kleur aan te passen en sla deze op.</li>
</ol>

<H2>Stap 4: </H2> 
<ol>
<li> Ga in Arduino naar File > Examples > Adafruit IO Arduino > Adafruitio_14_neopixel en maak een nieuw example aan. </li>
<li> Ga in de Arduino naar het tabje in de example naar ‘config.h’en plak je Adafruit IO username en Key erin bij IO_USERNAME en IO_KEY. </li>
<li> Doe hetzelfde met je wifi netwerk + wachtwoord in WIFI_SSID + WIFI_PASS. </li>
<li> Ga terug naar het vorige tabje: adafruit_14_Neopixel.ino en verander #define PIXEL_PIN 5 aan naar #define PIXEL_PIN D5.</li>
</ol>

<H2>Stap 5: </H2>
<ol>
<li> Verbind jouw ledstrip met de computer doormiddel van de board en upload je code. Als deze helemaal geupload is, ga je naar je serial monitor (rechts bovenin) en zet je deze op 115200 baud (Dit kan je in de dropdown links selecteren). </li>
<li> Als alles goed verlopen is verspringt de ledstrip naar de kleur die je gekozen had op de Adafruit.IO wesite. Wil je de kleur nog een keer aanpassen? Ga dan terug naar asafruit.IO website -> Dashboard -> naar de colorpicker en verander de kleur. Vergeet deze niet op te slaan! </li>
</ol>


<H2>Stap 6: </H2> 
<ul>
<li> Je hebt een Philips HUE gemaakt! :D </li>
</ul>
