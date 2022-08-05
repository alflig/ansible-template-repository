
**1. CD into /vagrant and type vagrant up**  <br />
    $ cd vagrant && vagrant up 

**2. SSH into the controller node**  <br />
    $ vagrant ssh controller  <br />     
    
**3.Run script to create and distrubute keys** <br />
    $ cd /home/vagrant/ && bash key_gen.sh           

**3. Add vagrant as sudo user to run playbooks as vagrant**  <br />
   $ cd etc/ansible/playbooks && ansible-playbook -i ../hosts.ini add-sudo-user.yml
  
