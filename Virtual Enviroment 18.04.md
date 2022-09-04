### Install pip3

sudo apt-get install -y python3-pip

### to install package

pip3 install package_name

### setup few more packages and development tools

sudo apt-get install build-essential libssl-dev libffi-dev python-dev

### install venv module

sudo apt-get install -y python3-venv

### create a enviornments

python3 -m venv project_env

### Now create a virtual environment 

    virtualenv venv 

>you can use any name insted of **venv**

### You can also use a Python interpreter of your choice

    virtualenv -p /usr/bin/python2.7 venv
  
### Active your virtual environment:    
    
    source venv/bin/activate
    
### Using fish shell:    
    
    source venv/bin/activate.fish

### To deactivate:

    deactivate

### Create virtualenv using Python3
    virtualenv -p python3 myenv

### Instead of using virtualenv you can use this command in Python3
    python3 -m venv myenv
