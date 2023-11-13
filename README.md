# moderntoring

The project is a small example of a monitoring solution using Prometheus, AlertManager, and Grafana. 

By default, the node-exporter is used. All of the basic metrics are available through it. The remote-write is used to send metrics to the main administrator's server.

Change the configs accordingly to your needs.

Deployment is automated using Ansible.

$ ansible-playbook -i inventory setup.yml

After that you can login into Grafana on http://your-server-ip:3000 (credentials are admin/admin)

In Grafana, configure Prometheus as a data source with the URL http://your-server-ip:9090.
