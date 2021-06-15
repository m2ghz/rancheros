# rancheros
what cloud-config.yaml code can do?
1-resize disk
2-configure network setting such as ip and gateway for specific interface
3-disable debug,autologin and password features
4-change ssh port
5-add sample public ssh-key
6-config nfs client, before config this, you should enable volume-nfs first

add node-exporter with prom.yaml
first you should move prom.yaml file to this directory:
/var/lib/rancher/conf/cloud-config.d/
then:
ros service create prom.yaml
ros service enable prom.yaml
reboot


@dwsclass dws-ops-009-rancheros
