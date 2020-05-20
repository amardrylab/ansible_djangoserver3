# Django Server generation on Google Cloud Platform
## First Clone the repository into your local machine

git clone https://github.com/amardrylab/ansible_djangoserver3.git

## Second run the code in your local machine

- cd ansible_djangoserver3
- ansible-playbook instance_djangoserver.yml

## Third login to your remote server

ssh www.drylab.in

## Fourth Create a virtual environment

virtualenv myproject

## Fifth Activate the virtual environment

source myproject/bin/activate

## Sixth Change directory

cd myproject

## Seventh Install Django

pip install django

## Eighth Create and new Project

django-admin startproject myproject .

## Nineth Put your website name in the myproject/setting.py

ALLOWED_HOST = ['www.drylab.in']

## Tenth Restart the nginx and uwsgi

- sudo service nginx restart
- sudo service uwsgi restart
