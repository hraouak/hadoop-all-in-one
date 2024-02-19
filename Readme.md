sudo apt-get update
sudo apt-get upgrade -y
sudo apt-get install ansible -y
sudo apt-get install git -y
git clone https://github.com/hraouak/hadoop-all-in-one.git
cd hadoop-all-in-one\ansible
ansible-playbook main.yml

