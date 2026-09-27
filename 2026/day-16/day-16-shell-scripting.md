TASK 1: First script
#!/bin/bash

echo "Hello, Devops"

TASK 2: variables 
name="Fuzail"
role="Devops engineer"

echo "Hello, I'm $name and I am a $role"

TASK 3: Taking input from user
#!/bin/bash

read -p "Enter your name" name
read -p "Which is your favourite tool" tool

echo "HELLO $name , your favourite tool is $tool"

TASK 4.1: If-Else Condition
#!/bin/bash

read -p "Enter your Number : " num

if [ $num -lt 0 ]
then echo "Number is negative"

elif [ $num -eq 0 ]
then echo "Number is zero"

else
echo "Number is positive"

fi

TASK 4.2: Checking file if it exists
#!/bin/bash

read -p "Enter the file name : " file

if [ -f "$file" ]
then echo "File found $file"

else
        echo "File not found "
fi

TASK 5: Final task of the day

#!/bin/bash


service_name="nginx"

read -p "Do you want to check the status?(y/n)" reply

if [ "$reply" == "y" ]

then sudo systemctl status $service_name

elif [ "$reply" == "n" ]
then echo "Skipped"

else
        echo "invalid response"
fi


Things I have learned today :

1. Just start does not matter even if you don't know anything or you do not like. I started this where I did not know anything now I can create these scripts and still lot more to learn.
2. Have to watch closely with the Braces and Spaces cause that is where most error lies.
3. For the final task I used documentation and the help of gpt because the final task was showing results even if I was entering different alphabets, the reason was I did not put the spaces in IF statement.
