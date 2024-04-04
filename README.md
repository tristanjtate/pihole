# Pi-hole Setup Guide

Welcome to the Pi-hole setup guide! Follow these simple steps to set up Pi-hole, a network-wide ad blocker, on your Raspberry Pi.

## Technologies Used:

- **Pi-hole:** A network-wide ad blocker that runs on Raspberry Pi.
- **Raspberry Pi:** A versatile single-board computer used to host Pi-hole.

## Items Needed:

- **Raspberry Pi:** Any model of Raspberry Pi (e.g., Raspberry Pi 3 or Raspberry Pi 4).
- **microSD Card:** A microSD card (8GB or larger) to host the Pi-hole software.
- **Power Supply:** A power adapter to provide power to the Raspberry Pi.
- **Network Connection:** A local network connection (Ethernet) to connect the Raspberry Pi to your router.

## Steps:

1. **Prepare Raspberry Pi:**
   - Flash a fresh installation of Raspberry Pi OS Lite (Raspbian) onto the microSD card using Raspberry Pi Imager or Etcher.
   - Insert the microSD card into the Raspberry Pi and connect it to your router via Ethernet.
2. **Install Pi-hole:**
   - Open a terminal on your Raspberry Pi or SSH into it from a remote computer.
   - Run the following command to install Pi-hole:

     ```bash
     curl -sSL https://install.pi-hole.net | bash
     ```

   - Follow the on-screen prompts to complete the installation process.
3. **Configure Pi-hole:**
   - After installation, open a web browser on any device connected to your network and navigate to `http://<Raspberry_Pi_IP_Address>/admin`.
   - Follow the on-screen setup wizard to configure Pi-hole settings, such as upstream DNS servers and blocklists.
4. **Monitor Pi-hole:**
   - Once configured, you can monitor Pi-hole through its admin website.
   - Access the admin interface by navigating to `http://<Raspberry_Pi_IP_Address>/admin` in a web browser.
   - Here, you can view statistics, manage settings, and monitor network activity.

5. **Set Up Router DNS:**
   - Access your router's admin interface and change the DNS settings to use the IP address of your Raspberry Pi running Pi-hole.
   - This step varies depending on your router model, so refer to your router's documentation for specific instructions.
6. **Enjoy Ad-Free Browsing:**
   - Once configured, Pi-hole will start blocking ads network-wide, providing ad-free browsing experience for all devices on your network.

## Troubleshooting:

- **Unable to Access Admin Interface:** If you're unable to access the Pi-hole admin interface, ensure that you entered the correct IP address in the web browser and that Pi-hole is running correctly on your Raspberry Pi.
- **DNS Issues:** If you experience DNS resolution issues, double-check your router's DNS settings and ensure they point to the correct IP address of your Raspberry Pi running Pi-hole.

## Additional Resources:

- [Pi-hole Documentation](https://docs.pi-hole.net/)
- [Pi-hole Community Forums](https://discourse.pi-hole.net/)
- [Pi-hole Reddit Community](https://www.reddit.com/r/pihole/)
