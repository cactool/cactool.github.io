# Step by Step Guide: Running Cactool on MacOS
*This guide was based on MacOS Ventura (v13.4.1), and should be mostly the same on other versions*

The primary way most users will be setting up the Cactool platform will be through their normal work machine. These guides are designed for these users in mind. The process to set it up might seem a little inconvenient when compared to other apps, but trust me, it’s actually quite easy! It requires a few prerequisites, but this guide goes through them. 

The method of installation in this guide will be via Docker. Docker allows for some pretty neat virtualisation options, but all you really need to know is that it allows you to install and start Cactool relatively straightforwardly in a way which keeps it separate from all your other files.

## 1. Download & Install Docker

Docker has their own guide for installing Docker for Mac here: [https://docs.docker.com/desktop/install/mac-install/](https://www.docker.com/)

To download Docker, go to [https://www.docker.com/](https://www.docker.com/) and download the most current version for your machine. Double check which type of Apple Machine you have, either Intel or Apple Silicon based machine, as each will need a different version of the program.

 When downloaded, install Docker. This should take enough time for you to grab a coffee.

<picture><img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/eb123c19-9ad4-47d4-944c-691ced22c7f0"></picture>
  
<picture><img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/416c43e8-4790-4ea4-9a5d-d6e00753dc42"></picture>


 

When you’ve installed, it, open up Docker from your Applications folder. Keep this open in the background, we will need it later.



## 2. Install Python
MacOS does come with a version of Python3, but it’s generally not recommended. So, pop over to https://www.python.org/downloads/ to download a version. It’s a similar process to Docker. Download the file and open it.


## 3. Installing Cactool

With Docker and installed, open a Terminal. To do this, go to “Go” on your Tool bar, and click on “Utilities” as blow, you can then find Terminal here. 

<picture><img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/9f370a43-2f9f-47c9-8012-a25426b29fdb"></picture>
<picture><img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/55a5088d-c720-4238-8bbf-c713fd1c0f18"></picture>


 

Alternatively press Command + Space, and type Terminal.


Next we want to download Cactool (woop), this is easy. Simply type (or copy and paste in) in the below
```
git clone https://github.com/cactool/cactool
```
<picture><img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/3aa5b6d6-9ed6-489d-b89a-632fdfc20b7a"></picture>


Your system will automatically download all the needed files!



## 4.Running Cactool

Now, go back to Terminal and go to the file where Cactool is installed
  
```
cd cactool
```
  

Let’s tell Docker we’ve got a program we want it to use, and to start it up for us. Enter in the below command:
```
docker-compose up -d
```

<picture><img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/22b86131-0bc3-4034-b251-3b80e3a10f54"></picture>



Docker will go through the process of installing a Cactool for you from the previously downloaded files, it will then start up Cactool for you! Amazing right? If you go back to Docker Desktop, you should be able to see Cactool running. 

<picture><img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/35f90e0f-9f61-4c0d-a3a4-c999c8fd1c06"></picture>


From Docker Desktop, you can start and stop Cactool. You will need to start Cactool from Docker when your computer restarts.

To make sure Cactool is running, you can go to http://localhost:80/ (when running the default configs) in your browser, and see Cactool running.

To stop/restart Cactool, open up Docker, go to Containers, and press the Start/Play icon. Do not delete the container at any point unless you have finished your use of Cactool, or you will lose your data.

<picture> <img width="500" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/7a8afb14-19cb-4cfc-a24f-30c26f645153"></picture>


Congratulations, you now have a working version of Cactool! You can now start working on your project, or make additional configuration changes (some of which are especially important if you want to work outside of your network)
