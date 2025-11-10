#  Deploy & Monitor a Next.js Project on an AWS EC2 

````
by Md Khurshed Alam Nayem
(Batch 7)
(10 November, 2025)
````

*   EC2 Setup
    -   EC2 Region in Mumbai
        ![GitHub Logo](images/step-1.png)
    -   EC2 instance tag name "nayem-ec2-module3"
        ![GitHub Logo](images/step-2.png)
    -   create key pair as RSA type generated which is "nayem-module3"
        ![GitHub Logo](images/step-key-pair.png)
    -   OS Ubuntu
        ![GitHub Logo](images/step-3.png)
    -   set security group where SSH allowed only
        ![GitHub Logo](images/step-4.png)
    -   set 30GB storage
        ![GitHub Logo](images/step-5.png)
    -   assign instance 1 & launch
        ![GitHub Logo](images/step-6.png)
    -   connect EC2 instance
        ![GitHub Logo](images/step-7.png)
*   Environment Setup
    -   from my Mac Terminal
        ![GitHub Logo](images/step-8.png)
    -   run sudo apt update
        ![GitHub Logo](images/step-9.png)
    -   run sudo su & apt install nodejs npm
        ![GitHub Logo](images/step-10.png)
    -   check versions
        ![GitHub Logo](images/step-11.png)
    -   git clone https://github.com/mdarifahammedreza/next-japan.git
        -   I got a folder as next-japan
        ![GitHub Logo](images/step-12.png)
    -   Install PM2 globally
        ![GitHub Logo](images/step-13.png)
*   Project Deploymen
    -   Install project dependencies using npm install
        ![GitHub Logo](images/step-14.png)
    -   EC2 security group update
        ![GitHub Logo](images/step-15.png)
    -   PORT=3001 pm2 start npm --name "ec2-nextjs" -- run prod
        ![GitHub Logo](images/step-16.png)
    -   project running on http://3.110.170.117:3001
        ![GitHub Logo](images/step-17.png)
*   Monitoring and Management
    -   pm2 list
        ![GitHub Logo](images/step-18.png)
    -   pm2 logs
        ![GitHub Logo](images/step-19.png)
    -   pm2 monit
        ![GitHub Logo](images/step-20.png)
    -   Set up PM2 to automatically start the project on server reboot(pm2 startup)
        ![GitHub Logo](images/step-21.png)



