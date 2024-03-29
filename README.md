# Cooking Blog Web Application

This document provides hosting detail of the cooking blog item catalog application.

## Host
```
IP Address: 54.218.100.75
SSH Port: 2200
```

### Remote Access
```
ssh -i ~/.ssh/grader grader@54.218.100.75 -p 2200

# Note: Private key for user grader is provided with submission notes.
```

## Live URL
http://www.54.218.100.75.xip.io/

## Software Stack 
```
AWS lightsail Ubuntu Instance
Apache2
git 
mod-wsgi
python2.7
postgresql
```

## Configuration Changes

#### AWS Lightsail / Linux
- Enabled TCP port 2200
- Enabled NTP port 123
- Disabled SSH port 22
- Created user `grader` and enabled sudo access
- Added authorized key for ssh access

### Installation
- Copied application to `/var/www/html`
- Initialized postgres database

### Apache2 Configuration
- Updated WSGI path and addess wsgi script for applicartion under `/var/www/html`

## Python Dependenices
```
flask
Flask-SQLAlchemy
Flask-HTTPAuth
Jinja2
httplib2
oauth2client
packaging
psycopg2
requests
SQLAlchemy
```

## Reference

- https://github.com/nehakalbhore/udacity-itemcatalog-cooking-blog
- https://stackoverflow.com/
- Google OAuth APIs
