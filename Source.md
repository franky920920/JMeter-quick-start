# Apache JMeter quick start guide for unicorn server

## [Recommend] Run JMeter on AWS  (With dynamic password)
1. Launch an EC2 instance:
    - AMI ID: `ami-031ad1c39789278cd`
    - Instance type: `t3a.xlarge` or larger
        (If you're using AWS educate, use `t2.2xlarge`)
    - Security Groups: Allow RDP (TCP port 3389) from your IP or Anywhere
    - Key pair: use your own key pair.
2. Connect to this instance using its public IP address and the following credentials: 
    - User: `Administrator`
    - Password: Get dynamic password from AWS console
3. Run `jmeter.bat` on the desktop.
4. In the JMeter application, click on `file` > `open` and navigate to the `example.jmx` file located on your Desktop. Then click `open`. (If an unexpected error occurred, just ignore it.)
5. Open `Example`> `Thread Group` > `HTTP Request` from left panel
6. Set your endpoint URL on this page.
    - Protocol: `http`
    - ServerName: `<ELB>.<region>.elb.amazonaws.com`
    - Path `/calc?input=SUNhbkhhelVuaWNvcm4%2FLTg5OTk%3D`
7. Start testing! Enjoy!

## Run JMeter on AWS  (With static password)
1. Launch an EC2 instance:
    - AMI ID: `ami-010afa1805c0d889e`
    - Instance type: `t3a.xlarge` or larger
        (If you're using AWS educate, use `t2.2xlarge`)
    - Security Groups: Allow RDP (TCP port 3389) from your IP or Anywhere
    - Key pair: use your own key pair or proceed without key pair.
2. Connect to this instance using its public IP address and the following credentials: 
    - User: `Administrator`
    - Password: `.t9JK.N(T3vEzP-eU5xpBLE=N3.O8nn5`
3. Run `jmeter.bat` on the desktop.
4. In the JMeter application, click on `file` > `open` and navigate to the `example.jmx` file located on your Desktop. Then click `open`. (If an unexpected error occurred, just ignore it.)
5. Open `Example`> `Thread Group` > `HTTP Request` from left panel
6. Set your endpoint URL on this page.
    - Protocol: `http`
    - ServerName: `<ELB>.<region>.elb.amazonaws.com`
    - Path `/calc?input=SUNhbkhhelVuaWNvcm4%2FLTg5OTk%3D`
7. Start testing! Enjoy!

## Run JMeter on local Windows Machine
1. Install Java [Direct download link](https://javadl.oracle.com/webapps/download/AutoDL?BundleId=244036_89d678f2be164786b292527658ca1605 "Download Java")
2. Download Apache JMeter [Zip](https://downloads.apache.org//jmeter/binaries/apache-jmeter-5.4.1.zip "Download Zip") [Tgz](https://downloads.apache.org//jmeter/binaries/apache-jmeter-5.4.1.tgz "Download Tgz")
3. Extract Zip (Tgz) file
4. Download the sample config file [Example.jmx](http://cdn.rdto.io/Example.jmx "Example JMX")
5. Run `jmeter.bat` under `apache-jmeter-5.4/bin/`
6. In the JMeter application, click on `file` > `open` and navigate to your `example.jmx` file. Then click `open`. (If an unexpected error occurred, just ignore it.)
7. Open `Example`> `Thread Group` > `HTTP Request` from left panel
8. Set your endpoint URL on this page.
    - Protocol: `http`
    - ServerName: `<ELB>.<region>.elb.amazonaws.com`
    - Path `/calc?input=SUNhbkhhelVuaWNvcm4%2FLTg5OTk%3D`
9. Start testing! Enjoy!

--
Markdown source available at [https://github.com/franky920920/JMeter-quick-start/](https://github.com/franky920920/JMeter-quick-start/new/main "Github.com"). File issues there and contribute there.

Franky Chen (c) 2021
