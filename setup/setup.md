# Cactool: Installation Guide


#  In-depth step-by-step guides:

- [Step-by-step guide for installing Cactool on Windows]()

- [Step-by-step guide for installing Cactool on MacOS]()

- [Step-by-step guide for installing Cactool on RaspberryPi] ()

# Quick Installation Guide

You can install Cactool on your local machine or on a server through [Docker](https://www.docker.com/) or directly using [PIP (package manager)](https://pip.pypa.io/en/stable/). Running Cactool through a server is useful if you want to have multiple coders or want to code through your mobile while situated away from your main computer. 

[Cactool also has some custom build configurations](/setup/config)

## Docker

### 1. Install [Docker Desktop](https://www.docker.com/products/docker-desktop), and start it. 

### 2. Clone the repository

```bash
git clone https://github.com/cactool/cactool
```

### 3. Enter the cactool directory

```
cd cactool
```

### 4. Run `docker-compose`

Make sure the Docker is running then run

```bash
docker-compose up -d
```

An instance should be accessible on port 80

## Directly (with PIP)

### 1. Install Cactool

```bash
pip install cactool
```

### 2. Start the website

```bash
cactool
```

The server will be running on port 80 and configuration files can be found in the generated `docker-config` folder.


## Custom Builds
There are some additional configuration settings available. For example those aimed at low-memory machines (such as installing Cactool on a Raspberry Pi), or server users with a public facing instance (such as custom ports, limiting file size uploads, and limiting user-signups. [Please read the configuration guidance here.](/setup/config)




