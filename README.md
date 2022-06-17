# Prometheus Stack
<img src="https://prometheus.io/assets/favicons/android-chrome-192x192.png" width="200px"><img src="https://i.imgur.com/dgpIE5E.jpg" width="200px"><img src="https://cdn.icon-icons.com/icons2/2415/PNG/512/redis_plain_wordmark_logo_icon_146367.png" width="200px"><img src="https://dyltqmyl993wv.cloudfront.net/assets/stacks/node-exporter/img/node-exporter-stack-220x234.png" width="200px">
## This compose file includes everything Prometheus needs to run.
Make sure to check the ports as it is set to MY scheme, which may not work for you.
* The port on the left is the port on your server, the port on the right is the internal docker port
* Leave the port on the right alone, you are welcome to change the others as you need.

# Stack contents:
* Prometheus
* Node Exporter
* Cadvisor
* Redis

-------------------------------------

# Installation Notes:
* Copy all files to a directory of your choosing
> I use home/{username}/docker/{project-name}/
* Open the ```docker-compose.yml``` file and edit appropriately
> Please make sure to note the ports you choose and any other variables you want to change
* Open ```prometheus.yml``` and edit the IP/port of the machines you want to scrape data from
> The values in there now are for my docker host, you will need to change these IPs unless you lock your server to 192.168.1.5.
> Basically, just change the IP address to your server(s) IP address(es) unless you changed the ports too.
> Edit accordingly, just pay attention to what you're doing and you'll be fine.
* Open a terminal in this directory
* ``` sudo docker-compose down ```
* ``` sudo docker-compose up -d ```
> **Configuring Grafana, Telegraf, Prometheus, InfluxDB, and your dashboards is outside the scope of this readme.**
