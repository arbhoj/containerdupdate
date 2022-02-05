# Update Containerd Configuration

This repo contains a simple ansible playbook to update containerd configuration.

Here are the steps to be performed to run this

1. Update inventory.yaml with the cluster host ip's or resolvable DNS names
2. Update var.yaml file with the registry infomation 
> Note:
> For `default_image_registry_mirrors` the entry for `docker.io` is required so do not omit it.
> The containerd config.toml file is defined as a jinja template in the templates dir. This makes it flexible. However, in case the requirement is to have a fixed defined config.toml then simply replace the templates contents with that file. Just make sure the name is the same.
