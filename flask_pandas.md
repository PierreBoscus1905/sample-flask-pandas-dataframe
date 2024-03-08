Pour installer docker : 

git clone  https://github.com/<votre_repo_perso>/docker-aston-poec.git
cd docker-aston-poec
python3 -m venv venv  # set up the module venv in the directory venv
source venv/bin/activate  # activate the virtualenv python
pip install --upgrade pip
pip3 install wheel  # set for permissions purpose
pip3 install ansible # install ansible
pip3 install requests # extra packages
ansible --version # check the version number # should be the latest 2.13.x
ansible-playbook -i inventory playbook.yml # run the playbook for installing docker


