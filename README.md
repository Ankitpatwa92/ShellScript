# ShellScript
Basic Syntax and commands

#### How to declare variable in shell script
varName=value
age=5

#### Declare array in shell script
my_array= ("1" "2" "3" "yes" "no")

#### if else condition in shell script
```
##### simple if
if [ $age == "5" ]
then
   echo yes he is eligible
fi

##### if with else

if [ $age == "5" ]
then
   echo "Yes, He is eligible"
else 
 echo "No, He is eligible"
```

#### Get array length
```arraylength=${#arrayName[@]}```


#### iterate over array
```
for (( i=1; i<${arraylength}+1; i++ ));
do
	echo ${myArray[i]}
done
```

#### write executable command
```eval your_command```

#### for loop
```
for ( i=1; i<5; i++ )
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

echo $folderName   output  drakula

echo ${!folderName}   output amit
```
#### Check for empty or undefined
```
if [ ! -z "$KAFKFA_URL" ]
then
  echo "Please assign Kafka Variable"
fi  
```

#### Run Script in Debug Mod
```add `set -x` at begning of script```

#### Append value in variable result
```"${varName} myAppendValue"```
