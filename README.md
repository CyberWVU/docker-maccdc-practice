MACCDC Practice
===========================

This is a docker-compose file to help practice for MACCDC.
It contains:
* Big Blue Button
* Cyclos
* Cyclos DB
* Nagios
* Request Tracker 4

At the moment Big Blue Button needs some tweaking.


Running:
---------------
1. Install [docker](https://docs.docker.com/engine/installation/), [docker-compose](https://docs.docker.com/compose/install/)
2. Clone this repo, cd to it
3. docker-compose up (Add -d to have everything run in the background)

To bring everything down, ctrl+c if not detached, otherwise docker-compse down if in detached mode.

That's it. It will take some time to download all the images and have everything come up.

Access
---------------
Anywhere $IP is mentioned, that is your internal IP on linux, or docker vm on windows/linux (docker-machine ip default)

#### Big Blue Button:
* http://$ip

#### Cyclos:
You will need a Cyclos account to setup and configure it.
*  http://$ip:8080

#### Nagios:
* http://$ip:8001/nagios/
* Username: nagiosadmin
* Password: admin

#### Request Tracker:
* http://$ip:8010
* Username: root
* Passowrd: password
