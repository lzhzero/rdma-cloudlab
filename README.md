scripts to deploy infiniband support on cloudlab use UBUNTU16

currently focused on Mellanox and QLogic HCAs


install_cloud_key.sh  //connectivity
install_ansible_latest.sh //ansible environment

make changes to inventory.ini for ips

ansible_playbook env_setup.yml to setup mellanox infiniband environment
(the last step of driver reload may caues lost of connectivity on some Cloudlab server, manual reboot required)

ansible_playbook env_setup_qlogic.yml to setup Qlogic invironment

ansible_playbook install_herd.yml to install herd

ansible_playbook install_erpc.yml to install eRPC
