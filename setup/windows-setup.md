# Step by Step Guide: Running Cactool on Windows 10.

*This guide is based on Windows 10, but  should be mostly the same on Windows 11.*
  
The primary way most users will be setting up the Cactool platform will be through their normal work machine. These guides are designed for these users in mind. The process to set it up might seem a little inconvenient when compared to other apps, but trust me, it’s actually quite easy!
  
The primary method of installation in this guide will be via Docker. Docker allows for some pretty neat virtualisation options, but all you really need to know is that it allows you to install and start Cactool relatively straightforwardly. 
  
  
## 1. Installing Docker
Docker has their own guide to installing Docker for Windows here: [https://docs.docker.com/desktop/install/windows-install/](https://docs.docker.com/desktop/install/windows-install/)

### Optional
Older versions of Docker may require you to enable Windows Subsystem for Linux (WSL) to work. We recommend you first try without enabling WSL, but enable it if required during the Docker install. In Windows 10, go to your search bar and type “Turn Windows Features On and Off” and click on the on the returned result.

<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/e516bdf8-42e8-4b97-adc1-ac2c471a62ff"></picture>

Then in Windows features, scroll down to “Windows Subsystem for Linux” and enable this. You might need to restart your machine.

    
### Downloading and Installing Docker
To download Docker, go to (https://www.docker.com/)[https://www.docker.com/] and download the most current version. When downloaded, install this. This should take enough time for you to grab a coffee.


<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/a2930c3d-08df-48b2-85a6-a56662fda355"></picture>  
 
<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/8b81a2f7-e339-4669-a5c1-48f464aaa336"></picture>


When this is complete, Docker should be installed on your machine, you can search for it in your search bar. Start the program.
  
<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/359a0e3d-f32b-4e00-b708-d569cdbef323"></picture>
  
    
## 2. Installing Git
The next thing you’ll want to do is install Git. This allows us to quickly pull Cactool from Github and onto your machine. You can install it from here: https://git-scm.com/download/win
  
<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/69adcbce-5a74-474c-a693-3c25817c86a8"></picture>
  
 

This is an easy install.
  
  
## 3. Installing Cactool
  
Finally, with both Docker and Git Installed, we can get onto the fun stuff! With Docker open, go to your search bar again and open up the Command Prompt.  

Once there, you can install Cactool quickly through the following command:

```
git clone https://github.com/cactool/cactool
```
    
<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/77775528-018a-4036-9bcb-78d6e099126f"></picture>  

<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/60e9c81e-00a1-4066-a166-42aaa8a89a78"></picture>  

<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/d30ad9e2-0334-47c5-97e1-83f0f9653b23"></picture>  

  
   

 

## 5. Running Cactool

Nice! Now let’s go to the place where we have installed Cactool in the terminal itself, this can be done through

```
cd cactool
```

Now we want to tell Docker that we have Cactool ready for it to use, and for it to start an instance up for us. To do this we type in and hit Enter:

```
docker-compose up -d
```
 
 <picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/d90661a3-85b7-412a-916a-ed54a777427b">.  </picture>

<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/e2abc16f-a53e-442d-b53d-934ecfd6118c">  </picture>

<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/62031cd4-6118-480a-8c6d-300ebe5c7bf3">  </picture>

 


Docker will then nicely start an instance of Cactool up for us! If you go back to Docker Desktop, you should be able to see Cactool running.

<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/e9916b25-a930-4dbc-97fc-c168a71b5eb6"></picture>. 

 

From Docker Desktop, you can start and stop Cactool. You will need to start Cactool from Docker when your computer restarts.


To make sure Cactool is running, you can go to http://localhost:80/ (when running the default config) in your browser, and see Cactool running.

<picture><img width="400" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/8d14ca62-b9f2-4321-b355-3148d1344bb0"></picture>

To stop/restart Cactool, open up Docker, go to Containers, and press the Start/Play icon. Do not delete the container at any point unless you have finished your use of Cactool, or you will lose your data.
   
  
**Congratulations, you now have a working version of Cactool!**
You can now start working on your project, or make additional configuration changes (some of which are especially important if you want to work outside of your network)
