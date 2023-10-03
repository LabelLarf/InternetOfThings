# InternetOfThings

<H1> LEDstrip kleur via een colorpicker in via Adafruit IO </H1> 


Stap 1: Instaleer de library Adafruit IO Arduino in de Arduino applicatie. Tools -> Manage labraries

Stap 2: Ga naar https://io.adafruit.com/ en maak een gratis account aan. Als deze is aangemaakt ga je naar https://io.adafruit.com/overview 
(Dit was voor mij niet duidelijk, als het niet te vinden is, ga in google en zoek Adafruit overview. Dan kom je op de goede pagina terecht.)

Stap 3: Klik op de pagina de gele sleutel aan en kopier je username en key. Maak vervolgens een dashboard aan, onder kopje dashboard en klik 'nieuw dashboard aanmaken.'
Geef het een naam en een discriptie. Sla deze vervolgens op. Klik op het dashboard en maak een nieuw blok aan. (Dit is het tandwieltje) Kies uit de lijst de colorpicker en maak een nieuwe feed aan die je 'Color' noemt. Sla dit op en selecteer de Color feed en klik op Next STep. Geef het block een leuke optionele titel en creeer het blok. Klik vervolgens in het dashboard op de color picker om hiervan de kleur aan te passen en sla deze op.

Stap 4: Ga in Arduino naar File > Examples > Adafruit IO Arduino > Adafruitio_14_neopixel en maak een nieuw example aan. Ga in de Arduino naar het tabje in de example naar ‘config.h’en plak je Adafruit IO username en Key erin bij IO_USERNAME en IO_KEY. Doe hetzelfde met je wifi netwerk + wachtwoord in WIFI_SSID + WIFI_PASS. Ga terug naar het vorige tabje: adafruit_14_Neopixel.ino en verander #define PIXEL_PIN 5 aan naar #define PIXEL_PIN D5.

Stap 5:Verbind jouw ledstrip met de computer doormiddel van de board en upload je code. Als deze helemaal geupload is, ga je naar je serial monitor (rechts bovenin) en zet je deze op 115200 baud (Dit kan je in de dropdown links selecteren). Als alles goed verlopen is verspringt de ledstrip naar de kleur die je gekozen had op de Adafruit.IO wesite. Wil je de kleur nog een keer aanpassen? Ga dan terug naar asafruit.IO website -> Dashboard -> naar de colorpicker en verander de kleur. Vergeet deze niet op te slaan!


Stap 6: Je hebt een Philips HUE gemaakt! :D
