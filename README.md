
**1. CD into /vagrant and type vagrant up**  <br />
    $ cd vagrant && vagrant up 

**2. SSH into the controller node**  <br />
    $ vagrant ssh controller   <br />
    
    $ cd /home/vagrant/      

**3.Run script to create and distrubute keys** <br />
    $ bash cd /home/vagrant/ && key_gen.sh           

 
 
**3. Add vagrant as sudo user to run playbooks as vagrant**  <br />
   cd into etc/ansible/playbooks in the controller node to add vagrant as sudo user  <br />
   $ ansible-playbook -i hosts.ini add-sudo-user.yml
