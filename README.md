# SRE_Challange

There are 2 roles, 1 that will provision the EC2 instance - inorder for that to work you will need to set the vars within Defaults.

The 2nd role is the actual configuration role of the EC2 instance and it will deploy HTTPS over NGINX, for that to work you will need to update the IP of the actual EC2 instance within /dev/inventory.

To run the playbook make sure to be on the root folder and run : 

sudo ansible-playbook -i dev infra_main.yml
