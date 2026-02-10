# AWS EC2 Hands On Commands

This document contains all commands used during my hands on work with AWS EC2.
All commands were executed on an Ubuntu EC2 instance accessed through SSH.
This file serves as proof of real practical interaction with an EC2 server.

## SSH Connection to EC2

ssh -i youtube-key.pem ubuntu@PUBLIC_IP

## Verify Python Installation

python3 --version

## Check Current Directory

pwd

## Create Python File on EC2

nano app.py

## Run Python Script

python3 app.py

## Update System Packages

sudo apt update

## Install pip

sudo apt install python3-pip -y

## Verify pip Installation

pip3 --version

## Create Python Virtual Environment

python3 -m venv myenv

## Activate Virtual Environment

source myenv/bin/activate

## Install Python Library inside Virtual Environment

pip install pandas

## Verify Library Installation

python
import pandas
exit()

## Deactivate Virtual Environment

deactivate

## EC2 Instance Lifecycle Management

The EC2 instance was stopped from the AWS Console when not in use to reduce cost.
After completing the practice the EC2 instance was terminated to avoid further billing.

## Security Note

No key files credentials or sensitive information are included in this documentation.
All commands shown here are safe for public GitHub repositories.
