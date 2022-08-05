1. CD into /vagrant and type vagrant up

2.  # SSH into the controller node
    $ vagrant ssh controller   

    $ cd /home/vagrant/         
    # CD into the vagrants' home directory to distribute SSH keys to nodes
  
    $ bash key_gen.sh           
    # Run script to create and distrubute keys
 
 
3. # Add vagrant as sudo user to run playbooks as vagrant
   cd into etc/ansible/playbooks in the controller node
   $ ansible-playbook -i hosts.ini add_sudo_user.yml
