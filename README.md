# Pi-Hole-homelab-setup
Network-wide Ad Blocker Running On A Raspberry Pi 4 
Hardware 4GB RAM 32GB MicroSD , GiGABIT Ethernet
Base OS - Rasperry Pi Os Desktop edition *came pre installed* Swapped to CLI mode once Pi-Hole was up


Set up the PI-Hole in October 2025 running 24/7 since due to privacy concerns and wanting to have a little fun.

I first purchased the Pi from ThePIhut *great customer service*
The SD card already came flashed which was great but if you are needing to flash yourself its nice and simple grab yourself a 16GB or 32GB microSD with and adaptor load up Balena Etcher Software click flash and select the RasperryPi OS image *.img file* found on the Raspberry PI Website then slam it in the Pi and away you go with the setup.

after first boot load the terminal and do sudo apt update && upgrade it takes 2 minutes and stops half the future headaches later 

next run this command to install Pi-Hole in your terminal either through SSH *if you've enabled SSH right after boot* or directly on the machine curl-sSl https:://install.pi-hole.net

after the install finishes youll get a prompt for static or DHCP *dynamic host configuration protocol* you will want to select static simiply because if the ip is dynamic on every wakeup the pi hole will switch ip so you laptops , TVS and phones stop knowing where to find it which makes the pi-hole obsolete.

next i went to the web interface and changed the upstream DNS from Google to cloudflare at 1.1.1.1 simply because i care about privacy.

finally i added the domain blocklists these blocklists can been found in many places with a simple google search , Githubs the best place, have a look at what suits you *dont go overboard otherwise youll end up blocking more than you need*

*heres the live dashboard*


<img width="1240" height="879" alt="Screenshot from 2026-01-07 13-27-57" src="https://github.com/user-attachments/assets/cd9db539-dab4-492a-b11f-c5f539065f9c" />
