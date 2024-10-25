# Python and Deep Learning


* Follow the notebooks under **Basic Tools** section on [here](https://web.stanford.edu/class/cs224u/background.html).
* I found this [YouTube Channel](https://www.youtube.com/@coreyms/videos) very useful.


## Git and GitHub

* set a ssh key pair (public and private) for your machine and GitHub account.

## SSH Configuration

* SSH Connection
* Passwordless


## HPC

* set a ssh key pair (public and private) for your machine and HPC account.
1. 

   use `ssh-keygen -o -a 75 -t ed25519 -f ~/.ssh/keyname -C "email"`


2. test agent is running

	eval "$(ssh-agent -s)"

3. add new key to SSH agent

ssh-add ~/.ssh/keyname

4. copy ssh public key to remote

remote ip: HPC ip
username: Case ID

ssh-copy-id -i ~/.ssh/keyname.pub username@remote_ip

or copy 
cat ~/.ssh/keyname.pub
copy content to server in path: ~/.ssh/authorized_keys


