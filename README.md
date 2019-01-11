# ShellScript
Basic Syntax and commands

#### How to declare variable in shell script
```
syntax:  varName=value
age=5
```
#### How to take input in shell script
```
read myVar
```

#### Declare array in shell script
```my_array= ("1" "2" "3" "yes" "no")```

#### if else condition in shell script

###### simple if
```
if [ $age == "5" ]
then
   echo yes he is eligible
fi
```
###### if with else
```
if [ $age == "5" ]
then
   echo "Yes, He is eligible"
else 
 echo "No, He is eligible"
 fi
```

#### Get array length
```arraylength=${#arrayName[@]}```


#### iterate over array
```
for (( i=1; i<${arraylength}+1; i++ ))
do
	echo ${myArray[i]}
done
```

#### Write executable command
```eval your_command```

#### for loop
```
for (( i=1; i<5; i++ ))
do
	echo i
done
```

#### Replace character in string
```replacedVariable=${varName//_/-}  //Here _ is repalced by -```


#### Value of Value
```
drakula=amit

folderName=drakula

echo $folderName   //output  drakula

echo ${!folderName}   //output amit
```
#### Check for empty or undefined
```
if [ ! -z "$KAFKFA_URL" ]
then
  echo "This is kafka url localhost:9092"
fi  
```

#### Run Script in Debug Mod
```add `set -x` at begning of script```

#### Append value in variable result
```"${varName} myAppendValue"```


#### Curl Command Use
curl is used to download file
```
curl -o myFileName https://abc.com/dockerfile    //file be saved with myFileName
curl -O https://abc.com/dockerfile    //file be saved with name provied in url

```

#### Read file line by line linux
The -r option passed to read command prevents backslash escapes from being interpreted.
```
fileName=file.txt
while read line
do
    
	echo "Line from file $line"
	echo  "reading first word of line=>   $(echo  "$line" | awk '{print $1}')"
	echo  "reading second word of line=>  $(echo  "$line" | awk '{print $2}')"
    
done<$fileName 

```

#### Write Shell command in multiple line using backslash

```
curl -o myfile \
https://myorg.com/myfile
```

#### Replace Content inside file
```
sed -i.bak 's/string_to_replace/replace_with/' file.txt   //Single Occurance
sed -i.bak 's/string_to_replace/replace_with/g' file.txt  //All Occurance
sed -i.bak 's/^string_to_replace/replace_with/g' file.txt  //^ use for exac match  user and username are different 

```

#### Insert a line after pattern matching

```
sed '/pattern/a some text here' filename

sed -i.bak '/username/a This is my text' needtodelete.txt

if your file is following symlink
sed --in-place --follow-symlinks 's/cat/dog/' pet_link

```


#### Find a file in directory
```

find ./ -name '*abc.txt'

```
