# rpi-network-managment

Raspberry PI docker configuration to run Homepage, PI-Hole, Internet Monitoring &amp; Grafana.

## Launch the ansible script

Launch the script `ansible-playbook playbook.yaml -K -i inventory.yaml`
Launch a dry run `ansible-playbook playbook.yaml -K -i inventory.yaml --check`

## Security

Update WEBPASSWORD with the following command : `docker exec -it pihole pihole -a -p change-this-password`

## Ports exposition

53:tcp  PI Hole
53:udp  PI Hole
67:udp  PI Hole
80:tcp  PI Hole
3000    Homepage
3030    Grafana
9798    Speedtest

## See also

- https://github.com/geerlingguy/internet-pi
