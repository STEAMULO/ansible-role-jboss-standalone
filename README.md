JBoss AS v7.1.1-Final
==============

Installation d'un JBoss AS v7.1.1-Final

Requirements
------------

Nécessite un JAVA 6 minimum

Role Variables
--------------

Voici les variables disponibles avec leurs valeurs par défaut :

    # installation jboss
    jbossAdminUsername: jboss
    jbossAdminPassword: steamulo
    jbossBase: /usr/share/jboss
    jbossUser: jboss
    jbossAjpPort: 8009
    jbossHttpPort: 8080
    jbossHttpsPort: 8443
    
    # liaison de l'application steamengine avec le ROOT jboss si souhaité
    homeDir: null
    skipApplicationLink: false

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      vars:
        - homeDir: "/projet"
      roles:
         - { role: steamroles/jboss-standalone }

License
-------


Author Information
------------------

STEAMULO - http://www.steamulo.com