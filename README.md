This tutorial aimed at modifed Tozed-VN009 some information 

it will cover two drivers

1.Android spreadtrum

2.SPD_ Driver

How to use these driver depend on your own system and system type, such as Win10 x64
After installing the driver, best to restart the computer.

1.Power off the Vn009 ，connect the vn009 and pc with Type c data cable, then turn on the vn009

2.Open the device manager of the computer, and 5-6 AT COM ports will appear. Usually the first one (eg. COM6)

3.Then install the putty, "connection type" select Serial, and then select the corresponding COM port for the Serial line above. eg. COM6  Speed 115200
You can enter the AT command below to change the string

4.The method is very simple. The input content will not be displayed and will not affect execution. After the input is completed, simply press Enter. Prompt OK indicates successful execution

Change string command:

AT+SPIMEI=0, "861111111111111"

View modification results:

AT+SPIMEI?

U had better to restore the factory settings after successful modification
adb
user：superadmin
Password:lo que te dio la pagina de arriba (https://tool.zootu.cn/tools/api/007imei/)
login web como super usuario: en la shell poner este comando

cat /tmp/mdlcfg.sysconfig | grep SYS_SENIOR_LOGIN_PWD

Change string command:
atcmd 'AT+SPACTCARD=0'
atcmd 'AT+SPIMEI?'
atcmd 'AT+SPIMEI=0,"861111111111111"'
