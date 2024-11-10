##1. Start Vagrant
Before running the Ansible playbooks, you need to start the Vagrant environment. You can do this by navigating to your Vagrant project directory in your terminal and using the following command:
```
vagrant up
```
This command will start the virtual machines defined in your Vagrantfile.

##2. Configure Inventory
You have the following inventory configuration:

```
[dbserver]
192.168.80.12

[webserver]
192.168.80.13
```

Make sure this is saved in a file named inventory.ini (or similar) and specify this inventory file when running your Ansible playbooks. 
##3 execute playbook in order to deploy service 

```
ansible-playbook -i inventory playbooksql.yml //for mysql server
ansible-playbook -i inventory playbook.yml // for webserver 
```
after that check eachport server are ready to use and configuration is set 
![image](https://github.com/user-attachments/assets/d1d59503-e04f-4af8-a918-576afc3bd86d)
![image](https://github.com/user-attachments/assets/361e28af-56c3-4562-9e38-af1287426d01)
