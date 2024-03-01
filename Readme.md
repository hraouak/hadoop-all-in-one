sudo apt-get update
sudo apt-get upgrade -y
sudo apt-get install ansible -y
sudo apt-get install git -y
git clone https://github.com/hraouak/hadoop-all-in-one.git
ansible-playbook -vvv hadoop-all-in-one/ansible/before_restart/main.yml
sudo reboot
ansible-playbook -vvv hadoop-all-in-one/ansible/after_restart/main.yml

