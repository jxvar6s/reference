Enable remi-repo on CentOS 7

This is what I found online for enabling remi-repo in order to install a different version
of php. In my case, my system went from php54 to php56. Do not forget to have sudo privileges
for using YUM package manager. Check remi-repo documantation for more advance configurations
at https://rpms.remirepo.net

+ Download epel-release

  $ yum install -y epel-release

+ Download remi-repo.

  - Note: cd into your directory of choice and enter the following command.

  $ wget https://rpms.remirepo.net/enterprise/remi-release-7.rpm

+ Install the remi-repo.

  $ rpm -Uvh remi-release-7.rpm

              OR

  $ yum install http://rpms.remirepo.net/enterprise/remi-release-7.rpm

+ Install the following command package to access yum-config-manager command.

  $ yum install -y yum-utils

+ Enable the repository.

  $ yum-config-manager --enable remi-php56

+ Update the system.

  $ yum update

+ Checking php version and available extensions.

  $ php --version
  $ php --modules
