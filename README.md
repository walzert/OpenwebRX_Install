# OpenwebRX_Install



sudo su -i

add-apt-repository -y ppa:myriadrf/drivers

apt-get install soapysdr-tools  python3-soapysdr python3-numpy rtl-sdr soapysdr-module-rtlsdr hackrf soapysdr-module-hackrf 

wget https://www.sdrplay.com/software/SDRplay_RSP_API-Linux-3.07.1.run

./SDRplay_RSP_API-Linux-3.07.1.run


wget -O - https://repo.openwebrx.de/debian/key.gpg.txt | apt-key add

echo "deb https://repo.openwebrx.de/debian/ buster main" > /etc/apt/sources.list.d/openwebrx.list

apt-get update

apt-get install openwebrx

