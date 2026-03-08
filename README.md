# Campus Occupancy AIoT Project

Tämä projekti seuraa kampuksen täyttöastetta MQTT-sensorin ja MongoDB-tietokannan avulla.

## Node-RED Flow
Ohjelma löytyy tiedostosta `node-red-flow.json`. Se sisältää:
- MQTT-vastaanottimen
- Datan muokkauksen (Function node)
- Tallennuksen MongoDB Atlas -pilvipalveluun
- Dashboard-visualisoinnin
