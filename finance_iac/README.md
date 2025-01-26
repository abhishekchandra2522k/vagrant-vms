## Vagrant VM via Provisioning

1. Provisioning can be done using Vargant file and httpd service in the CentOS VM. Find the commands below:
2. yum install httpd wget unzip vim -y
   systemctl start httpd
   systemctl enable httpd
   mkdir -p /tmp/finance
   cd /tmp/finane
   wget https://www.tooplate.com/zip-templates/2133_moso_interior.zip
   unzip -o 2133_moso_interior.zip
   cp -r 2133_moso_interior/\* /var/www/html/
   systemctl restart httpd
   cd /tmp/
   rm -rf /tmp/finance
3. Put this in provisioning, make sure private IPs are enabled.
4. Access the website from the IP
