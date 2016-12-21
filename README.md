# Ubuntu set up script

Steps required:

1. Set up ssh keys  

2. Install git and ansible:

  1. `sudo add-apt-repository ppa:git-core/ppa`
  2. `sudo add-apt-repository ppa:ansible/ansible`
  3. `sudo apt update`
  4. `sudo apt install git ansible`

3. Get this ansible playbook:

  `git clone https://github.com/rpbaptist/ubuntu-setup.git ~/.ansible`

4. Set the vault password file:

  `vault-pass.txt`

4. Run ansible:

  `ansible-playbook ~/.ansible/main.yml --vault-password-file vault-pass.txt`
