### Admin user

Go to [**DOMAIN**](__DOMAIN__) to create the first user.
❗The **first** user created will have administrator rights; the following ones will be regular users.

### Configuration

The settings panel allows you to edit the following parameters:

* SMTP relay for sending emails
* File import size limit
* AWS storage
* AI models

### Application generation

Applications created with Baserow can be deployed on subdomains of [**DOMAIN**](__DOMAIN__).
By default, these subdomains will not be covered by a certificate recognized by browsers.
To make them accessible via HTTPS, follow these steps:

* create the subdomain corresponding to the application in YunoHost and install a Let's Encrypt certificate on it
* install the *Redirect* app in `reverse_proxy` mode and make it point to [http://127.0.0.1:__PORT_FRONTEND](http://127.0.0.1:__PORT_FRONTEND)__
