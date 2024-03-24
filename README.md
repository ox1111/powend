
# powerd exploit : Sandbox escape to root for Apple iOS < 12.2 on A11 devices

## 저자 commnet

if you want to debug the exploit just uncomment MEMDBG/MEMDUMP,
if you want to debug the ROP chains enable LOCAL_EXP, 
and if someone wants to port it to another device or wants to chain 
it with a kernel bug to have a tfp0, I'll be glad to help

![8](8.jpg)


and of course the exploit can work on 
all iDevices including iOS10.x,11.x with some slight modifications.


Apple fixed two nasty sandbox escapes
bugs I reported in iOS CVE-2019-8549 & CVE-2019-8552 ,
full exploit of CVE-2019-8549 will be released soon in coordination with 
@SecuriTeam_SSD



The exploit demonstrates how to get powerd's
task port by bootstrapping a fake service and communicate with it via ROP/JOP
