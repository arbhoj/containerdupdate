# Update Containerd Configuration

This repo contains a simple ansible playbook to update containerd configuration.

Here are the steps to be performed to run this

1. Update inventory.yaml with the cluster host ip's or resolvable DNS names

2. The containerd config.toml file is defined as a jinja template in the templates dir. This allows defining any templatized 
