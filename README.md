
**1. CD into /vagrant and type vagrant up**
    $ cd vagrant && vagrant up 

**2. SSH into the controller node**
    $ vagrant ssh controller   
    
**3. Run script to create and distrubute keys**
    $ cd /home/vagrant/       

  **4.Run script to create and distrubute keys**
    $ bash key_gen.sh           

 
 
**3. Add vagrant as sudo user to run playbooks as vagrant**
   cd into etc/ansible/playbooks in the controller node
   $ ansible-playbook -i hosts.ini add_sudo_user.yml
