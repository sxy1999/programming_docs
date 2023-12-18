# Install JDK 21 in Rocky Linux

First, edit the repo file

>sudo vi /etc/yum.repos.d/adoptium.repo

Then, paste the following and save the repo file.

```text
[Adoptium]
name=Adoptium
baseurl=https://packages.adoptium.net/artifactory/rpm/rocky/8/x86_64
enabled=1
gpgcheck=1
gpgkey=https://packages.adoptium.net/artifactory/api/gpg/key/public
```
Now run the yum command to install the openjdk 21

>sudo yum install temurin-21-jdk
 
To switch java version

>sudo alternatives --config java
