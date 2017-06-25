# udfsndfp.com
### Information
The important details of this deployment are as follows:
1. URL: [http://udfsndfp.com](http://udfsndfp.com/)
2. IP: 45.55.151.24
3. SSH port: 2200

### Third party software
The folowing programs were used to configure/run this server:
1. Apache2
2. Mod-wsgi
3. PostgreSQL
4. Pip
5. Psycopg2
6. SQLAlchemy

### Python packages
The following python packages were used in the web application:
1. Flask
2. Flask-SQLAlchemy
3. OAuth2client
4. Requests
5. Httplib2

### Configurations
The following configurations were made to the server:
1. Disable root login and password authentication
2. Change SSHD listen port to 2200
3. Set UFW to default deny incoming, allow outgoing, allow ports 2200, 80, and 123, and enable
4. Add apache2 'sites-available' conf file for the item catalog website
5. Run a2ensite udfsndfp.com.conf and a2dissite 000-default.conf to set apache to serve website
6. Edit /etc/sudoers.d files to give sudo access to users
7. Created PSQL role `weblink` to allow connection from web app
8. Used my `dbinit.py` file to initialize database and configure tables

