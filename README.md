# ansible-splunk

This is an automation installation of Splunk Universal Forwarder on windows hosts. You can use it to upgrade to a certain version or if the forwarder is not installed, simply, install it.
You have to set some variables to use this playbook. Follow these steps

## Steps

### 1. set the version that you want to install
example : 
splunkdesiredversion: 8.0.3
Note: you must just set the version you want without any quotation

### 2. set the splunk user name 
splunkuser: admin
It usually is admin

### 3. set the splunk password
splunkpasswd: 123456

### 4. If you use the deployment server to control and manage forwarders, you can set this in this section.
deploymentserver: 192.168.1.1:8089

you can set either IP or URI for this section, and you must set the port that usually is 8089, which is the default management port of Splunk. If you have changed it in your installation environment you must set it base on that.
