# Pi-hole-on-Windows-11
How to Install Pi-hole on Windows 11 using Docker

# Download and install Docker for Windows
Download Docker for Windows.There used to be a requirement to create a Docker
account, but luckily this is no longer required for personal use.
![Screenshot (88)](https://user-images.githubusercontent.com/111239341/221732727-4912e836-519d-4800-8ad6-386fab6450e2.png)

Once downloaded, install Docker. Make sure to leave the “Install required Windows
components for WSL 2” option ticked

![image](https://user-images.githubusercontent.com/111239341/221733150-303734d1-1d03-4246-bb8e-eefc128ba599.png)

After installing you will need to reboot. Once your computer restarts, Docker should
automatically start.

![3-docker-complete-wsl2-installation](https://user-images.githubusercontent.com/111239341/221733507-f3c7fec1-fb5d-494d-b516-4a44c3e8d1b9.png)

If you don’t already have WSL 2 installed, you may be prompted to download and install it separately from the Microsoft Website.

This is a small download and the installation completes very quickly. Once this is done, head back to Docker and click “Restart”. Docker should now be ready to use.

Docker will present you with a tutorial. Either walk through the tutorial, or click skip if you want to dive right in.
# Download Pi-hole
To download the Pi-hole container, open Windows Command Prompt as an administrator and type the following command: docker pull pihole/pihole Pi-hole will now download into a Docker container.
# Give your PC a static IP address
The next step is to give your Windows PC a static IP address so it can be reliably reached on your network. To do this, head to Windows Settings (right click on the start button and click “Settings”).

1. Select “Network & internet” from the sidebar menu.
2. Click on WiFi, (or Ethernet if you’re using a wired connection). Then click on the network properties item. This will most likely be prefaced with your network name.
3. Half way down the page, click “Edit” alongside IP assignment.
4. This will launch the “Edit network IP settings” dialog. Select manual from the dropdown list.
5. In the dialog that pops up, set a manual IP address.
