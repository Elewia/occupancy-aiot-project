# Campus Occupancy AIoT Project

Tämä projekti hyödyntää MQTT-dataa sekä logeja että generoitua kulkudataa hyödyntämällä.

## Node-RED
Ohjelmaan on luotu pipeline, joka hyödyntää kävijädataa Robo Garagelta sekä vertaisanalysoituna generoitua kulkudataa.
Dataa syötetään yksinkertaistettuna ja suodatettuna Mon Node-RED dashboardille reaaliaikaiseen kuvaajaan sekä omaan MongoDB Atlas clusteriin.

## Google Colab
Ohjelmaan syötetään kulkuhistoriadata sekä Robo- että AIoT Garagen kulkutunnistimista.
1. Kulkudatasta on piirretty kuvaaja, jossa on näkyvissä suurimmat päivittäiset samanaikaiset kävijämäärät molemmista tiloista samaan kaavioon viimeisen kahden kuukauden ajalta. Saman kaavion osalta on myös piirretty kävijäennusteet seuraavan kuukauden ajalle, perustuen kokonaisuudessaan aiempaan kerättyyn dataan.
2. Node-red ohjelman kautta MongoDB Atlakseen tallennetusta datasta tehty kuvaaja viimeisen 24h tallennetun tiedon perusteella (ensimmäiset tallenteet 8.3. klo 19 aikoihin)
Ylimääräisinä kuvaajina
- Monte Carlo -viuhka kuvaamassa Robo garagen mahdollisia käyttöennusteita seuraavalta kuukaudelta
- heatmap-kuvaaja garagejen yleisimmistä viikottaisista käyttötunneista
- kävijämäärien liukuvat keskiarvot garageilta
