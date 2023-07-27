# Configuring Cactool
**Both Docker & PIP install Routes**

For most single-user projects, the typical install guides should be sufficient for your own use. That pathway allows you to use Cactool within your own network.

In other use-cases (such as sharing Cactool with multiple users), you will want to make some configuration changes. These are designed for a range of use-cases. For example, for using Cactool on low-memory machines (such as installing Cactool on a Raspberry Pi), or server users with a public facing instance (such as custom ports, limiting file size uploads, and limiting user-signups. 

There are also settings which allow you to stop the creation of new user accounts on your instance (important for putting Cactool out in the public or in large networks).




# How to edit configuration values
--------------------------------------

### Docker Users
Changing config values can be done by directly editing the config file, “config.json” which can be found in the Cactool folder -> docker-config. Normally you will need to right-click this file and edit with a text editor (such as Notepad on Windows, or TextEdit on MacOS). 

You can find the Cactool folder in the place you installed Cactool. For example, if following the guide, MacOS users will find this in your home user directory. 


### PIP Users
For users installing Cactool though the PIP route, you can set config values in Terminal/Command Prompt with by running:

```
cactool set NAME VALUE
```

On some systems, this maybe be:
```
python -m cactool set NAME VALUE
```

Set values can be retrieved via cactool 

```
get NAME
```

The NAME will be given for each setting below.

In both pathways, you will need to restart your Cactool instance for changes to take effect.



# Available Settings
--------------------------------------


## Email domains
--------------------------------------
NAME: ```email-domains```

Only allows users to signup when using a specific email domain, such as liverpool.ac.uk. No @ is required. This has limited functionality at the moment and isn’t a recommended change.

 

## Instance Name
--------------------------------------
NAME: ```instance-name```

This allows you to change the name of the instance, and this is shown when using Cactool. For example, changing this to ‘The University of Liverpool’ will show ‘The University of Liverpool’ on your screen when using Cactool. This is especially useful when dealing with multiple instances of Cactool on the same network. 
 


## Port
--------------------------------------
NAME: ```port```

Port numbers are ways to identify specific processes which an internet or other message can be forwarded to when it arrives at given server. By default, Cactool runs on the default port for websites, and there should be no reason to change it unless you’re running Cactool on a server infrastructure. 
 


## Unused settings
--------------------------------------
The below settings you may find in your config folder relate to a yet-to-be-enabled future feature set. As such you should leave these blank for now.

```request-email```  

```require-2fa```  

```require-email```  

  





## Secret Key – DO NOT MODIFY
--------------------------------------
Cactool automatically generates a 512-bit secret key when the server is first run. There is no need to modify this secret key to make it memorable as it is only used internally to cryptographically sign data and authenticate users. Shortening the secret key makes it guessable jeopardising the security of the server.
  


## Password protecting user signups
--------------------------------------
NAME: ```signup-code```

To prevent external unknown users from creating accounts on the Cactool instance or to restrict account creation to authorised individuals, you can set up a signup authorisation code that requires users to enter a password before creating an account on the server instance.

By default, if no signup code is entered or the signup code provided is empty, no code will be required while creating an account on the server. 

It is best practice to set a sign-up code. If you are going to expose your instance outside your network, it is important you set a sign-up code. If you’re on a larger internal network (such as a university) you may wish to set a signup code anyway. 
  


## Limiting file upload size
---------------------------------------
NAME: ```upload-limit```

Strict file size upload limits can be set to prevent any service loss from any large files being sent over that the network or the server is unable to handle.

This value is Megabytes. By default, the upload limit is 1024 (or 1GB) and if necessary, the very strict default limit can be increased or decreased. This will likely be needed when using Cactool’s photo feature.

  

## Using HTTPS
------------
It is considered best practice to use HTTPS when handling requests, and some browsers will give warning flags for content served over HTTP. Using a reverse proxy can be used to allow Cactool to be served using HTTPS this can be done through applications such as ‘nginx <https://www.nginx.com/>`_ and `Apache <https://http.apache.org/>`_.

