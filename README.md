red hat Linux ---(casesensitive )
sudo(super user do)

file permission--
symbolic-
read-
Write-
Execute-
+-permit
- -deniy
u-users
g-group
o-others
a-all
chmod u+x,g+Wx,o+wx hello.txt

numeric
read-4
write-2
execute-1
chmod-6-userpermission44 hello.txt

umask
user mask -creation mode mask
0-7 octal no

directory
777
-022 unmask value     044
                     =733
=755

file
666
-0022 unmask value
622 default permission for file

one file add user and different permission
getfacl filename   exa getfacl doc.txt
adduser            adduser srushty

setfacl -m user:permision filename  example
setfacl -m srushty:rwx  doc.txt

for user--
useradd username
adduser username

for password--
passwd username 
password 

for delete user account
deluser username
userdel username(only user delete)
userdel -r username(profile delete with user delete)

for id--full permission roo id 0
command id.
id username(0-999 reserve se create andnother our statrt with 1000)

group account
addgroup/groupadd groupname
(deparment devide thats vay we create group,collection of user account)
useradd bu1(user)
passwd bu1(password)

usermodify
usermod -a(add) -G(group) groupname username(adduser)

group(which group member)
su(switch user) username
groups

show group
sudo groups
exit

add user multiple groups
usermod -a -G groupname groupname username

show group of list(for users accounts information)
getent group

show pacific group info
grep groupname /etc/group(file info)

cat /etc/passwd

show group and user validity 
cat /etc/shadow (all accounts show password encryption)/in windows SAM

which user is currently logedin
id usename

Linux change username UID userID







