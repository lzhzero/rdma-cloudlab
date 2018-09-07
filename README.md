scripts to deploy infiniband support on cloudlab use UBUNTU16

currently focused on Mellanox HCAs, will implement QLogic later

install_cloud_key.sh  //connectivity
install_ansible_latest.sh //ansible environment

make changes to inventory.ini for ips

ansible_playbook env_setup.yml to setup mellanox infiniband environment

ansible_playbook install_herd.yml to install herd

