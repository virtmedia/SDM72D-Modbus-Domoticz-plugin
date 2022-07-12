# SDM72D-Modbus
SDM72D-Modbus 3-fase power meter with RS485 Port modbus RTU plugin for domoticz

Original code bij MFxMF for the SDM630-M power meter https://github.com/MFxMF/SDM630-Modbus

Requirements: <br>
Working Domoticz instance with working python plugin service (see logs in domoticz)<br>
If python plugin service is not working try "sudo apt-get install python3.7 libpython3.7 python3.7-dev -y"<br>
<br>
Installation: <br>
cd ~/domoticz/plugins<br>
git clone https://github.com/bbossink/SDM72D-Modbus-Domoticz-plugin <br>
Restart domoticz: systemctl restart domoticz.service <br>
<br>
Configuration: <br>
Select "Eastron SDM72-D-Modbus" in Hardware configuration screen<br>
If needed modify some parameters (defaults will do) and click add<br>
Hint: Set reading interval to 0 if you want updates per "heartbeat" of the system (aprox 10s in my case)<br>
<br>
9 new devices will be automatically added. Go to devices tab, there you can find them<br>
Tested on domoticz v2020.2
<br><br><br>
Used python modules: <br>
pyserial -> https://pythonhosted.org/pyserial/ <br>
minimalmodbus -> http://minimalmodbus.readthedocs.io<br>
