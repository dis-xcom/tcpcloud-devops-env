# tcpcloud-devops-env

Clone the repo
==============
git clone https://github.com/dis-xcom/tcpcloud-devops-env
cd ./tcpcloud-devops-env

Install requirements
====================
pip install -r ./requirements.txt

Get cloudinit image
===================
wget https://cloud-images.ubuntu.com/trusty/current/trusty-server-cloudimg-amd64-disk1.img -O ./trusty-server-cloudimg-amd64.qcow2

Export variables
================
export ENV_NAME=tcpcloud-mk20
export IMAGE_PATH=./trusty-server-cloudimg-amd64.qcow2

Create and start the env
========================
dos.py create-env ./tcpcloud-wk20.yaml
dos.py start "${ENV_NAME}"
