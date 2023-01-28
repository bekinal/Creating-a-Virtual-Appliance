<h1>Creating a Virtual Appliance</h1>

<h2>Description</h2>
Project consists of creating a virtual appliance that can be used later without full configuration.
<br />


<h2>Utilities Used</h2>

- <b>VirtualBox</b>
- <b>Windows Server 2012</b>
- <b>BGInfo</b>

<h2>Creating a Windows Server 2012 R2 VM:</h2>
A Windows Server 2012 VM is created in VirtualBox. The GUI option is selected:<br/>
<img src="https://imagizer.imageshack.com/img922/9352/gNOfgP.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The installation proceeds until our machine is ready:<br/>
<img src="https://imagizer.imageshack.com/img923/378/b9YOhc.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The sysprep tool is run. Enter System Out of Box Experience (OOBE) is selected. We set the machine to reboot once the process is complete:<br/>
<img src="https://imagizer.imageshack.com/img922/8089/6rXl87.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Downloading BGInfo:</h2>
The BGInfo tool is downloaded to demonstrate that the software is saved to the virtual appliance. BGInfo is a Sysinternals tool that displays the machine's state in the background. First, the virtual machine is configured with NAT internet connectivity:<br/>
<img src="https://imagizer.imageshack.com/img923/739/UOAt86.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The server manager is opened, and IE Explorer Enhanced Security Configuration is navigated to:<br/>
<img src="https://imagizer.imageshack.com/img924/9697/GgtG0B.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Administrator IE ESC is set to off:<br/>
<img src="https://imagizer.imageshack.com/img922/4025/A4qjPA.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Internet Explorer is then opened:<br/>
<img src="https://imagizer.imageshack.com/img924/9249/LYGEDl.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Don't use recommended settings is selected:<br/>
<img src="https://imagizer.imageshack.com/img922/156/PyWkxf.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
BGInfo is downloaded from the microsoft website:<br/>
<img src="https://imagizer.imageshack.com/img924/1639/C4ph36.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The file BGInfo.zip is saved:<br/>
<img src="https://imagizer.imageshack.com/img923/9754/zfgTCU.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The files are moved to the C: directory. BGInfo64 is run with default configuration:<br/>
<img src="https://imagizer.imageshack.com/img924/1949/3fqcWi.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Default config is viewed, OK is selected to proceed:<br/>
<img src="https://imagizer.imageshack.com/img924/1015/HptO17.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The sysprep tool is opened, set to OOBE again, and set to shutdown upon completion:<br/>
<img src="https://imagizer.imageshack.com/img922/9858/0XF4Rh.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Launching the OCI:</h2>
The Windows Server 2012 machine is right-clicked. Export to OCI is selected:<br/>
<img src="https://imagizer.imageshack.com/img924/373/5RfuQS.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The format is set to Open Virtualization Format 2.0, and the directory is changed to documents:<br/>
<img src="https://imagizer.imageshack.com/img922/126/eJni3w.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Import appliance is used to test the .ova file that was exported:<br/>
<img src="https://imagizer.imageshack.com/img923/6310/Xlsdbx.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The virtual appliance opens in Out-of-Box Experience mode and allows the configuration of settings that were skipped earlier:<br/>
<img src="https://imagizer.imageshack.com/img922/7650/HfiU3n.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After going through basic setup, the C: directory is navigated. BGInfo is located, confirming that the appliance worked as intended:<br/>
<img src="https://imagizer.imageshack.com/img923/7404/iv80lU.png" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
