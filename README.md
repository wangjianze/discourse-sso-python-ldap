discourse-sso-python
====================
* This project is based on [discourse-sso-python](https://github.com/welenofsky/discourse_sso_python)

Requirements
------------
* Install python3
* Install ldap and jinja2 modules for python3 using easy_install or pip
* Install nginx/lighttpd with SSL (you don't want to transmit credentials over regular HTTP)

Steps
-----
* Place the contents of this project in the root directory of your webserver
* Modify the SSO url in the admin settings of Discourse
* Flow
** User clicks "Log In"
** Discourse redirects you to "https://my-sso-url?sso=SOMETHING&sig=ANOTHER-THING"
** You redirect the user to login screen, verify the auth. On success, redirect the user base to discourse


