# Prometheus Stack
This compose file includes everything Prometheus needs to run.
Make sure to check the ports as it is set to MY scheme, which may not work for you.
* The port on the left is the port on your server, the port on the right is the internal docker port
* Leave the port on the right alone, you are welcome to change the others as you need.

# Stack contents:
Prometheus
Node Exporter
Cadvisor
Redis
