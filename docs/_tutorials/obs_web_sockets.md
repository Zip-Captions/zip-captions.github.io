---
title: Using ZipCaptions with OBS to add Live Captions to your streams
description: ZipCaptions will connect with OBS using Web Sockets to allow you to add Live Captioning to your streams
layout: default
---
<h2>Using ZipCaptions with OBS to add Live Captions to your streams</h2>

To use this feature there are some steps that you will need to follow in both ZipCaptions, and in OBS. Before we begin you need to ensure that you have the following:

1. ZipCaptions open in a supported web browser
2. OBS (Open Broadcaster Software) [Download Here](https://obsproject.com/){:target="_blank"}{:rel="noopener noreferrer"} for Windows, Mac or Linux

Once you have your pre-requisites out of the way you then need to set up OBS

1. Open OBS and click on the **Tools** menu and then **Web Socket Server Settings**
![Opening the Tools Menu](/assets/obs_tools.png)

2. In the window which opens, check the box **Enable WebSocket Server** set a port which you can use (the default is **4455** and should be fine), and click **Generate Password**.
![Setting up the WebSocket Server](/assets/obs_socket_setup.png)

3. Now click on the **Show Connect Info** button and copy the _Password_ shown in the box by clicking on the **Copy** button next to it.
![Copying the Password](/assets/obs_password.png)

4. Now close the box and go to your browser window with ZipCaptions in it. Click on the **Broadcast/Sharing** button at the top of the screen, or in the menu bar.
![Opening ZipCaptions](/assets/zip_welcome.png)

5. Click **Yes I'm Sure** to the warning box, letting you know that you'll be sharing your captions.
![Accept the permissions](/assets/zip_permissions.png)

6. Scroll down the page until you get to the **Connect to Third Party Services** section, and expand it.
![Open the ZipCaptions Third Party Services Pane](/assets/zip_3rd_party.png)

7. Set the **Server IP** to _localhost_ (unless you're running OBS on a different computer to ZipCaptions, in which case you would enter the IP address of the computer running OBS), set the **Server Port** to _4455_ (unless you chose a different port in the setup in OBS, in which case you should enter the port you chose), and finally paste the password that you copied from OBS into the **Password** box and click on the **Connect** button. _The Captioning will now automatically start_.
![Setting up OBS in ZipCaptions](/assets/zip_obs_setup.png)

8. You will now see at the top of the screen that OBS is connected. Once OBS is streaming the _idle_ label will change.
![OBS is connected to ZipCaptions](/assets/zip_connected_obs.png)

9. Leave ZipCaptions open and head back into OBS, you can now start your stream and the captions will be sent to the stream from OBS.

Depedning on the service that you are using you may need to tell it that you are sending captions with your stream. For example, YouTube Live requires you to check the Captions box before you start your stream. 

The captions that ZipCaptions outputs are in the 608 Format. You can see an example of the settings required for YouTube Live below:
![YouTube Live Captioning Settings](/assets/youtube_live_settings.png)