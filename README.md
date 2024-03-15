# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/beb316df-4a96-44f2-98a4-994d78b171a6)

cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e7e1fffb-a87e-4260-95c7-b9a5cea17a63)

### Display the content of the files
cat < file1
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/61f6a7f4-642e-4f2a-b73c-0b3a73bcbe6b)


cat < file2
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/721ecac7-04e8-469f-9c16-fb7f07b9a45b)

# Comparing Files
cmp file1 file2
## OUTPUT
 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/aba03a9c-a626-4222-b1aa-fd783d119802)

comm file1 file2
 ## OUTPUT

 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e4f277f0-94b9-4e83-b3a0-8bb88b1cec56)

diff file1 file2
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e1cda817-6f73-45d7-a730-6d8bde062c87)

#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/d7d33202-b150-4588-a9ba-6b81d1e6295f)

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/471fbb8a-4dd4-4b6e-a81e-93bcac6a7f1a)

cut -c1-3 file11
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/8a5cd67b-6120-4889-a3f7-3a76d1815e1c)

cut -d "|" -f 1 file22
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/5c67372b-0430-4c4a-875e-d8eabd1b848b)

cut -d "|" -f 2 file22
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/5b9e486f-3875-4382-8fe8-889972bb2767)

cat < newfile 
```
Hello world
hello world
^d
````
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/68c83a6d-3a61-49c0-aa4e-c92cd417cb3d)

cat > newfile 
Hello world
hello world

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/d4f6a4e1-2981-4e90-8869-407616d257ee)
 
grep Hello newfile 
grep hello newfile 
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/d17eaf4e-4d6c-4653-abde-6858901ff825)

## OUTPUT
grep -v hello newfile

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/f8f24f6b-4c82-4b4e-9240-9ad8ce149316)

## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e4327ec1-3a49-4741-919c-6cb745bb602b)

cat newfile | grep -i "hello"
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/bf7ca2d1-e81c-4f90-a7b8-4f2ba0a424db)

cat newfile | grep -i -c "hello"
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/11416445-322e-4656-8e45-9297992158e6)

grep -R ubuntu /etc
## OUTPUT

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/6047ff53-9ec8-481e-8575-c5ec3349beba)

grep -w -n world newfile   
## OUTPUT


cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/c1bc48d2-b926-451e-b993-e21e038791ec)

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/ec37f173-9342-4170-9d30-6ec867cbf1ba)

egrep -w 'Hello|hello' newfile 
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e090f52a-08f4-4c55-922e-8765a3d126f2)


## OUTPUT
egrep -w '(H|h)ello' newfile 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/652e18ab-a999-4dd3-8f2d-109a49957f92)


## OUTPUT
egrep -w '(H|h)ell[a-z]' newfile 
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/abcf6608-5828-44c9-80d9-14f8e16473ef)


## OUTPUT
egrep '(^hello)' newfile 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/207db60c-bc91-4178-aaa6-3b6886b5f82f)

## OUTPUT
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/5c8801b4-b0ed-4ae6-8baa-f43d276f8a3c)

egrep '(world$)' newfile 
## OUTPUT
egrep '(World$)' newfile 
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/8bdaaa42-e37a-4a46-a140-959477af06e3)


## OUTPUT
egrep '((W|w)orld$)' newfile 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/49db0010-678b-4530-ba66-a6ed0f3d09e0)

## OUTPUT
egrep '[1-9]' newfile 
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/cdf2d808-3d23-4f15-a383-1b12c03d0d95)


## OUTPUT
egrep 'Linux.*world' newfile 


## OUTPUT


egrep 'Linux.*World' newfile 
## OUTPUT
egrep l{2} newfile
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/fc0b8ebe-9937-4ba0-9548-c8c47f6ffb5d)


## OUTPUT
egrep 's{1,2}' newfile
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e761a581-4f5f-4213-9007-5f4961f5bbd8)


## OUTPUT 


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/c8a488cb-874d-4b25-8dde-219507e2c52e)


sed -n -e '3p' file23
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/3dd62e5d-6400-4ec0-a3da-13597bf1be71)


## OUTPUT
sed -n -e '$p' file23

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/db6f3955-e23e-4798-bb9b-95fc2372f2d5)

## OUTPUT
sed  -e 's/Ram/Sita/' file23
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/14aba2ed-adbe-4eb4-834b-8a7e809a4916)

## OUTPUT
sed  -e '2s/Ram/Sita/' file23
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/67d68790-a667-4777-b0c0-617301fd53de)


## OUTPUT
sed  '/tom/s/5000/6000/' file23

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e2f1c4bc-9e07-42ef-899c-68045139a3ab)

## OUTPUT
sed -n -e '1,5p' file23
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/f07344f9-3c38-4c7e-bdff-66d1c4d33a14)


## OUTPUT
sed -n -e '2,/Joe/p' file23

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/39677b68-53be-45c8-b1d9-a6b16f3494f8)

## OUTPUT
sed -n -e '/tom/,/Joe/p' file23

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/18a1018d-59ec-4a18-987e-795c018262c5)

## OUTPUT
seq 10 
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/bd90904c-9882-4818-8c19-879d272c908d)


## OUTPUT
seq 10 | sed -n '4,6p'

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/096ad40d-be2e-448e-b0c3-293fcc6ebbce)

## OUTPUT
seq 10 | sed -n '2,~4p'
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/0de28dc3-936d-4acf-8adf-362e3d89bcd2)


## OUTPUT
seq 3 | sed '2a hello'

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/54f3cbd5-8550-4de2-8348-e0f4e57311d9)

## OUTPUT
seq 2 | sed '2i hello'

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/ca688d39-d47c-4f87-9de9-98bee12467b5)

## OUTPUT
seq 10 | sed '2,9c hello'
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/745e57cf-1776-45a4-afcf-8dac28b7a2fe)


## OUTPUT
sed -n '2,4{s/^/$/;p}' file23
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/982f2679-71d1-453c-8264-5c0f4a87b1de)


## OUTPUT
sed -n '2,4{s/$/*/;p}' file23
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/86c55bfb-72f8-49e8-93ac-cbbad5d4ae7b)


#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/26d50d31-2f32-4ff9-beaf-79b69d8303ae)

## OUTPUT


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
```

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/aa4f908f-4ccc-4162-b3dc-17373bdb55d5)

uniq file22
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/3522efde-245c-427e-be16-912103281945)


## OUTPUT
#Using tr command
cat file23 | tr [:lower:] [:upper:]
 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/8ecfecd4-c95f-4467-9d6d-386288e800d4)

 
 ## OUTPUT

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/0872233a-6fb0-4d08-8326-b0ec317956a8)

cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/fa170933-9f18-424f-8115-69e6ce9ef40c)

cat urllist.txt | tr -d ' '
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/2de521bc-8cff-4fd4-805c-c978b8d8ac94)

 ## OUTPUT
cat urllist.txt | tr -d ' ' | tr -s '.'
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/934c2c2d-0131-4fe5-baef-af94074c8377)


## OUTPUT
#Backup commands
tar -cvf backup.tar *
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/83606077-90d9-479f-94bc-f82e22e24b66)


## OUTPUT
mkdir backupdir

mv backup.tar backupdir
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/d544ca7f-ba90-407c-a716-46136e4db86f)
 
tar -tvf backup.tar
 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/a0b57850-c01b-4023-bb30-455c1b5a5541)

## OUTPUT
tar -xvf backup.tar

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/0769d40b-a6c9-4a6e-8c08-ed12bffa3271)

## OUTPUT
gzip backup.tar

ls .gz

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/c7b7885a-7677-4594-ae2e-457ddbfff068)

## OUTPUT
gunzip backup.tar.gz

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/8a858afd-b41d-4160-a8ec-bd0dcc0a8277)

## OUTPUT
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/37b47c26-ee40-43bd-8c0b-7af7ab4cb598)


chmod 755 my-script.sh./my-script.sh

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/7d043e79-ce11-4e84-89c8-434dc0d171f8)

## OUTPUT

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/5a4327a9-f26e-4a69-9e14-dd7908d59a32)

cat herecheck.txt

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/529c19f4-72ae-44ca-b624-d3081e498dee)

## OUTPUT


cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/0dea6f69-d559-4576-bc87-eccdd842819c)

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/1c8cc3a2-a357-423c-9dff-444718c6bede)

chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/40a4717a-4294-434b-a7e6-78567e93884e)

## OUTPUT 
ls file1

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/2246da7d-8df8-4192-93f1-107ab440fac9)

## OUTPUT
echo $?

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/625a053c-3583-44df-acb1-cd8d162c22d3)

## OUTPUT 
./one
bash: ./one: Permission denied
 echo $?

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/740b0523-9d10-4141-836d-634e4ec8bfec)

## OUTPUT 
abcd
echo $?
 
 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/0f13fc6d-b950-4bcf-8361-167d52d0167d)

 ## OUTPUT

# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/d12d4749-0a39-47a3-8ef2-c0dd95fb0110)


## OUTPUT
chmod 755 strcomp.sh

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/3671b658-93f4-43ea-ab16-47613e1f6c9a)

 
./strcomp.sh 
## OUTPUT
# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/bbb96d31-7930-4574-a2ff-e985773f926d)

./psswdperm.sh

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/6e4db949-3dee-4830-a8dd-7af2df3f28e5)

## OUTPUT

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/b1cf78fe-4f3e-44b7-b482-e2cdc9d465da)


./ifnested.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/14bb3495-8bc9-4cba-833d-503a6ff4d0d5)

## OUTPUT

# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/305eb71e-69fc-426c-b959-2db512190404)

$ chmod 755 iftest.sh
 
$ ./iftest.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/a5ba2b0d-5a49-4b4d-937f-054ef28c2d3f)

## OUTPUT

# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/542f671f-00ea-420a-8966-f4ecf2c3a5e2)

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/b47a8623-1236-405e-9a2d-6eb547cc4a1d)

## OUTPUT

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e441e221-807f-44d1-86f6-f392a2fa1934)

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/0702e8d8-0930-4bf5-a8f6-6442dcd0843d)

## OUTPUT


# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/0b35ba16-2a2f-4112-96da-8d28d76c9719)

$ ./ifcompound.sh 
## OUTPUT

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/ef3fe135-008e-439b-8a4d-78b4205fee4e)

 
$ ./casecheck.sh 
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh

 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/3faeb014-8ba4-4114-a026-def5bf5b5436)

 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh

 ![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/dbbcadd4-ca74-4954-9ab2-5f81945da040)

 $ ./untiltest.sh
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/4a84e1f0-eb66-4644-a93b-c99d6ca76b00)

 
$ chmod 755 forin1.sh
 
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/dadeaea0-f650-4814-967f-f7bf3c87d09a)

 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/82f5c261-5530-4864-9a31-bb35247e584a)

 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/ca5d6cae-e05f-4f9f-a2f3-f4b24f606a62)

$ ./forin3.sh 
 
## OUTPUT
cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/bf52f3d8-80e3-4bda-ba79-f8d6fb319b3d)


![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/a0871c29-a89d-486b-bdfa-9bfa5f92f004)


## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/5fd6ed85-fba9-4702-8102-0b62036ebd93)

## OUTPUT

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/9d037211-002b-4127-b02e-1254172635ed)

## OUTPUT

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 

![image](https://github.com/tamizhselvan23013460/OS-Linux-commands-Shell-script/assets/150231370/e29294bd-c2cc-4078-bbcf-885a0ad6a37e)

 ## OUTPUT

 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 

## OUTPUT
 
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 


## OUTPUT



$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 

 
 ./funcex.sh 1 2

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 



# RESULT:
The Commands are executed successfully.
