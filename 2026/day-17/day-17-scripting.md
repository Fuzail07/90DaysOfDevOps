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




 
