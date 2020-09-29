---
layout: post
title: Getting Drupal Running on Amazon EC2
---

This is for me. This could also be for you. That's why I'm posting it.

I needed to get a fully functioning Drupal installation running on a Free Amazon EC2 cloud instance. I had to pull in multiple websites in order to do it. Interspersed are some bits of wisdom that I needed to know in order to get things like "Module Install" to work.

Getting it up and running
[http://www.thingaweek.com/how-install-drupal-amazon-ec2](http://www.thingaweek.com/how-install-drupal-amazon-ec2)

Using Putty to SSH on Windows?
[http://pinehead.tv/linux/connect-to-amazon-ec2-using-putty-private-key-o](http://pinehead.tv/linux/connect-to-amazon-ec2-using-putty-private-key-o)

Access your server through ssh:

~~~
ssh ec2-user@IP -i keyname.pem
~~~

did you email yourself the key?

~~~
chmod 400 keyname.pem
~~~
[http://stackoverflow.com/questions/8193768/trying-to-ssh-into-an-amazon-](http://stackoverflow.com/questions/8193768/trying-to-ssh-into-an-amazon-)

Setting up SFTP access
[http://matthom.com/archive/2011/09/01/setting-up-amazon-ec2-instances](http://matthom.com/archive/2011/09/01/setting-up-amazon-ec2-instances)

~~~
sudo su -
chown -R ec2-user /var/www/html
chmod -R 755 /var/www/html
~~~

Using Filezilla for SFTP?
[http://www.codestore.net/store.nsf/unid/BLOG-20111012-0812](http://www.codestore.net/store.nsf/unid/BLOG-20111012-0812)

chown -R apache:apache /var/www/html/sites
(allows drupal to install modules without FTP installed)

Updating Drupal:
[http://www.echoditto.com/blog/updating-your-drupal-site-using-drush](http://www.echoditto.com/blog/updating-your-drupal-site-using-drush)

~~~
drush up
~~~

### Nice optimizations
[http://www.diginmotion.com/faq/108-running-a-website-on-amazon-ec2.pdf](http://www.diginmotion.com/faq/108-running-a-website-on-amazon-ec2.pdf)

### Own your files on EC2
~~~
chown -R apache:apache /var/www/html/sites/default/files
chown -R apache:apache /var/www/html/sites/all
~~~


