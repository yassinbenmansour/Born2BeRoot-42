
# Born2BeRoot 42/21

Developed for Debian so i'm not sure that it will run properly on CentOS distributive. Anyway, PM me on Discord if its working on CentOS or you have a suggestion/issues: MMBHWR#0793

# monitoring.sh script
Known issues: 
1) Cron may refuse to running script on boot due to bug in Debian (https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=635473). How to fix? [https://bugs.debian.org/cgi-bin/bugreport.cgi?att=0;bug=635473;msg=70]. Good luck :)
Theres also another way to fix it in my rebootfix.txt file, but it may not work anyway...

# Please, DO NOT copie + paste this thing with emptiness in your eyes and blank in your head!
It's highly recommended to know what u use and how&why it works even if i leaved an explanation in commentary. At least, it will be usefull for YOURS and ONLY YOURS defense. Google&man all the commands listed here and read about it's options/parameters/etc. Be intellegent, be adaptive, be SMART. Know the tool you use.
Still, i haven't validated it yet but i'm 98% sure that it's working as intended. (The remaining 2% is disk space and ssh lol)

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
To make this works u need to [$ chmod +x monitoring.sh] (ofc lol). 
Please note that you should run script as root because journalctl won't
work from user without sudo.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
# How to use
First off [$ sudo crontab -e] (yep, you need sudo to make cron runnig script as root.[$ crontab-e] will open another file that will run your script as user). Set nano/vi as your text editor for cron and add next lines in your crontab file:
~~~~~~~~~~~~~~~~~~~~~~~~~~
@reboot /path/to/file/monitoring.sh
*/10 * * * * /path/to/file/monitoring.sh
~~~~~~~~~~~~~~~~~~~~~~~~~~
Dont forget that you should write FULL PATH TO FILE (no ~/*/etc.) due to cron's pecularity.

# walkthrough37.txt
Guide how to correctly setup and configure both Debian and software. Including bonus-part partition set up.
# evalknowledge.txt
Little Q&A from Subject and whattocheck as evaluator.

I hope it's done for now and only thing that left to add is my evaluation result.
