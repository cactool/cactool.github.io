
# Accessing Cactool outside your network for Multiple coders or coding on the go

Cactool is designed to be used not only on your host machine, but by a range of coders on the same dataset. Cactool is also mobile optimised – giving coders the option to experience content as users would (such as on public transport) for more spatially attuned content analysis approaches. 

The below will walk you through some of the options.


# Network Set up for using Cactool for Multiple Coders

By default, Cactool is available to other computers on your local network. This means if you’re at home, you can connect to your instance from multiple computers (or your mobile phone) provided you’re connected to the same router. You simply need to type in the hosts machine’s Local IP or Host Name, where you installed Cactool, into your browser from another machine.

-	How to find your computer’s host name (MAC) [https://support.apple.com/en-gb/guide/mac-help/mchlp1177/mac]( https://support.apple.com/en-gb/guide/mac-help/mchlp1177/mac)

-	How to find your computer’s host name (Windows) [https://computing.cs.cmu.edu/help-support/find-hostname]( https://computing.cs.cmu.edu/help-support/find-hostname)

If you want to access Cactool outside of your local network, there are two different approaches you may wish to take. Both require you to make changes to your router (some may not have all features), or through a third-party service. So please check the manual for your router.

-	Through a Virtual Private Network (VPN). VPNs allow you to connect to an outside local network. So you can be out at work, connect through a VPN to your home network (where your host machine) is located), and access Cactool as if you were at home. 

-	Port Forwarding. Port forwarding exposes your computer to the internet, and allows to anyone with your IP to access your instance of Cactool. This guide to port forwarding by Reddit user brianatlarge  is a useful starting point: https://www.reddit.com/r/HomeNetworking/comments/i7ijiz/a_guide_to_port_forwarding/


There are security considerations for both, so please follow best practice. But as a guide, if you’re running Cactool at home for a small team of trusted researchers, or for you to access while working remotely, a VPN will be your best option. If you are hosting Cactool on a paid-for server, please contact your webmaster who can advise.



## **IMPORTANT notice regarding signup codes!**

It is important that if exposing your instance of Cactool outside of your network, that you set up a sign-up code to stop unknown users creating and uploading data to your instance of Cactool. [You can read how to do this here.](https://cactool.github.io/setup/config).




# Giving Access to a Dataset within Cactool

When you have set up your network, you will need to have log-ins to Cactool created for each user.  When sharing datasets, only the account that created the dataset can edit the question types.


The process for sharing the datasets for coding is as follows:
1.	Go to your dataset after you have uploaded it to Cactool, and click Edit. On this page will see the coder invite link*, this is what you will need to copy and share with your coder. **It is important that the coder is already logged in when they try to use this code.** Do not refresh your page until this link is clicked.

**You will need to change the “localhost” in this link to either your local network IP, or external IP address – or the link won’t work for the recipient.*


2.	When the coder has used the link, the dataset will show up on their account, and the admin account will be able to see they are linked to the dataset.   

<picture><img width="600" alt="image" src="https://github.com/cactool/cactool.github.io/assets/11173283/e20b0e23-bec2-4fa2-ad1b-4f2f7e939657"></picture>  
*When the second user has successfully clicked on the link, you will see them added to the dataset*


3.	The admin account will also be able to set the row ranges. This is useful if you have multiple coders and want to split up the workload. For example, you may want one person to code rows 1 to 25, and another to code from 26 to 50.

Done! Your connected coders will have access to the dataset and can start coding. Please only share the invite link with trusted users.
