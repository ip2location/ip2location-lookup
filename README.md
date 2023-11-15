# IP2Location

## THIS IP2LOCATION LOOKUP HAS BEEN INTEGRATED INTO IP2LOCATION C LIBRARY. PLEASE VISIT [IPL2ocation C Library](https://github.com/chrislim2888/IP2Location-C-Library) FOR THE LATEST RELEASE

IP2Location is a tool allowing user to get IP address information such as country, region, city, 
latitude, longitude, zip code, time zone, ISP, domain name, connection type, area code, weather, 
mobile network, elevation, usage type, address type and IAB category by IP address (IPv4 or IPv6) from IP2Location BIN database. 

For more details, please visit:  
https://www.ip2location.com/free/applications  



### Installation

1. Download or clone this repository to your local machine.

   ```bash
   wget https://github.com/ip2location/ip2location-lookup/archive/master.zip
   unzip master.zip && rm master.zip
   cd ip2location-lookup
   ```

   

2. Download the latest IP2Location C library from https://github.com/chrislim2888/IP2Location-C-Library

   ```bash
   wget https://github.com/chrislim2888/IP2Location-C-Library/archive/master.zip
   unzip master && rm master.zip
   ```

   

3. Copy the `libIP2Location` directory from the C library.

   ```bash
   cp -r IP2Location-C-Library-master/libIP2Location .
   ```

   

4. Start compilation and installation.

   ```bash
   chmod +x autogen.sh
   ./autogen.sh
   ./configure
   make
   make install
   ```

   


Usage
-----
Query an IP address and display the result 

```
ip2location -d [IP2LOCATION BIN DATA PATH] --ip [IP ADDRESS]  
```



Query all IP addresses from an input file and display the result

```
ip2location -d [IP2LOCATION BIN DATA PATH] -i [INPUT FILE PATH]  
```



Query all IP addresses from an input file and display the result in XML format 

```
ip2location -d [IP2LOCATION BIN DATA PATH] -i [INPUT FILE PATH] --format XML  
```




Download More Sample Databases  
------------------------------  
```bash
wget https://www.ip2location.com/downloads/sample.bin.db25.zip
unzip samples-db25.zip
```




Support 
------- 
Email: support@ip2location.com  
URL: https://www.ip2location.com  
