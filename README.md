# OpenwebRX_Install

## Requirments
Faster than Pi 4 more user than 5
12V for using it in the shack/ outdoor

## System
Board based on J4125 Quadcore 128GB SSD and 8 GB RAM
Current board: 
https://de.banggood.com/Beelink-Gemini-M-J4125-Intel-Lake-Refresh-Processor-DDR4-8GB-128GB-SSD-1000M-LAN-5_8G-WIFI-bluetooth-4_0-Mini-PC-Support-Windows-10-p-1718331.html?akmClientCountry=DE&cur_warehouse=HK&ID=47184

Possible Outdoor alternative: 
https://www.minipc.de/catalog/il/2736

## Install process


// Login to super user

su -i

// update current system and install sudo + gnupg

apt-get update
apt-get install sudo gnupg

// add the driver / modules for different SDRs

add-apt-repository -y ppa:myriadrf/drivers

apt-get install soapysdr-tools  python3-soapysdr python3-numpy rtl-sdr soapysdr-module-rtlsdr hackrf soapysdr-module-hackrf 

// currently not working adding SDRplay

wget https://www.sdrplay.com/software/SDRplay_RSP_API-Linux-3.07.1.run

./SDRplay_RSP_API-Linux-3.07.1.run

// add the openwebrx-repo and install openwebrx after install it is accessible at 0.0.0.0:8073

wget -O - https://repo.openwebrx.de/debian/key.gpg.txt | apt-key add

echo "deb https://repo.openwebrx.de/debian/ buster main" > /etc/apt/sources.list.d/openwebrx.list

apt-get update

apt-get install openwebrx

