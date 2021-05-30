Sending warning letter

There are two ways to do it.
First one:  internal mail tool, not recommended.

Second one: external mail tool call mailx

install 
yum install mailx -y  --------- command

config 
open /etc/mail.rc file

add following info  to this file

set from=yourEmailAddress smtp=smtp.emailSite
set smtp-auth-user=yourEmailAddress smtp-auto-password=password
set smtp-auth-login

all done.


