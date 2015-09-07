# Docker cluster with GlusterFS volume driver

The hosts are defined in the file [swarm](swarm). The cluster is provisioned using the following command:

    ansible-playbook -i hosts gluster-cluster.yml --ask-vault-pass

(You need to know my vault password or overwrite the file [group_vars/swarm](group_vars/swarm) so it contains your own `glusterrest_password`.
