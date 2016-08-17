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
    jbossServiceName: jboss
    jbossUser: jboss
    jbossAjpPort: 8009
    jbossHttpPort: 8080
    jbossHttpsPort: 8443
    jbossOsgiHttpPort: 8090
    jbossRemotingPort: 4447
    jbossTxnRecoveryPort: 4712
    jbossTxnStatusPort: 4713
    jbossSMTPRemoteHost: localhost
    jbossSMTPRemotePort: 25
    skipApplicationLink: false

    # zip archive without root folder /!\
    jbossZip: https://s3-eu-west-1.amazonaws.com/steamansible-resources/jboss/jboss-as-7.1.1.Final.zip
    
    # link an application root folder if needed
    jbossApplicationScanPath: /xxx/yyy/zzz

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