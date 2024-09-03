## Server

1. Copy the content of this project in a folder named `dvb-i` on your local webserver.
2. Open `frontend/dvbi-common.js` and edit the `PROVIDER_LIST` variable. Use the IP of your local webserver.
3. Open `5g-mag/5gmag-service-list-offering.xml` and edit the `dvbisd:URI` tag using the IP of your local webserver
4. Open `5g-mag/5gmag-service-list.xml` and configure the right stream URLS

## Client (5G-MAG DVB-I Player)

You can either do the required changes before applying the Exoplayer patch or afterward:

### Before patch

1. Open `Exoplayer.patch` and
   edit `String landing_url = "http://10.147.67.219:3333/dvb-i/frontend/android/player.html"`. Point to your local
   webserver

### After patch

1. Open `WebviewActivity.java` and
   edit `String landing_url = "http://10.147.67.219:3333/dvb-i/frontend/android/player.html"`. Point to your local
   webserver

