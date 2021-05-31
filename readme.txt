Sending email with mailx

There are two ways to do it.
First one:  internal mail tool, not recommended. it is slow and may be indentified as junk mail

Second one: external mail tool called mailx

install 
yum install mailx -y  --------- command

config 
open /etc/mail.rc file

add following info  to this file

set smtp-use-starttls      # add this
set from=yourEmailAddress smtp=smtps://smtp.gmail.com:587
set smtp-auth-user=yourEmailAddress smtp-auth-password=password
set smtp-auth=login
set ssl-verify=ignore
set nss-config-dir=/etc/pki/nssdb/

there is a problem :
Error in certificate: Peer's certificate issuer is not recognized.

can not fix it

all done 


