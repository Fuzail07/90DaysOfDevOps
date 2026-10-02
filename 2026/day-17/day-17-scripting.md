Task 1: For Loop
#######CODE########
#!/bin/bash
#
#
#

for i in mango apple banana grapes orange
do 
        echo " $i "

done

########OUTPUT##########
ubuntu@ubuntu:~$ ./for_loop.sh 
 mango 
 apple 
 banana 
 grapes 
 orange 


Task 2: While Loop

#########CODE###########
#!/bin/bash
#
i=1
while [ $i -le 10 ]
do
        echo "$i"

  i=$(( $i + 1 ))


done

echo "done"

##########OUTPUT##########

ubuntu@ubuntu:~$ ./while.sh 
1
2
3
4
5
6
7
8
9
10
done

Task 3: Command-Line Arguments

###########CODE############

ubuntu@ip-172-31-0-159:~$ cat greet.sh
ubuntu@ip-172-31-0-159:~$ cat greet.sh
#!/bin/bash
echo "HELLO $1 , your favourite tool is $2"

##########OUTPUT##########
ubuntu@ip-172-31-0-159:~$ ./greet.sh fuzail docker
HELLO fuzail , your favourite tool is docker


2. Create args_demo.sh that: 
###########CODE############
 ubuntu@ip-172-31-0-159:~$ cat args_demo.sh
echo "This is the first arguement $1"

echo "This is the second argument $2"

echo "This is the 0th argument $0 (file name)"

##########OUTPUT##########

ubuntu@ip-172-31-0-159:~$ ./args_demo.sh Hello Doston
This is the first arguement Hello
This is the second argument Doston
This is the 0th argument ./args_demo.sh (file name)

Task 4: Install Packages via Script

###########CODE############
ubuntu@ip-172-31-0-159:~$ cat install_packages.sh
#!/bin/bash

package="nginx curl wget"
for i in $package
do
if      sudo dpkg -s "$package" &> /dev/null
then    echo " installed"
else sudo apt install $package -y
fi

done

##########OUTPUT##########

Summary:
  Upgrading: 0, Installing: 0, Removing: 0, Not Upgrading: 5
nginx is already the newest version (1.28.3-2ubuntu1.11).
curl is already the newest version (8.18.0-1ubuntu2.7).
wget is already the newest version (1.25.0-2ubuntu4.4).
Summary:
  Upgrading: 0, Installing: 0, Removing: 0, Not Upgrading: 5

Task 5: Error Handling

###########CODE############

#!/bin/bash

set -e
mkdir /tmp/devops-test || echo "Directory already exists"

##########OUTPUT##########

ubuntu@ip-172-31-0-159:~$ ./safe_script.sh
mkdir: /tmp/devops-test: File exists
Directory already exists
ubuntu@ip-172-31-0-159:~$


WHAT I LEARNED ?
1. always check for the braces and check for loops opening and closing conditions most of the error resides there.

2. i learned fixing the script on my own .

3. learned while loop and for loop from the basic and still a lot to learn

