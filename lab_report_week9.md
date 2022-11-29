# Code
```
set -e
rm -rf student-submission
git clone $1 student-submission

echo "successfully copy"
cd student-submission

if [[ -e ListExamples.java ]]
then
    echo "The file exist"
else
    echo "The file not found"
    echo "Maybe Wrong File Name"
    exit 1
fi


cd ../
cp -rf lib student-submission
cp -f TestListExamples.java student-submission

cd student-submission

ls 
if [[ -e TestListExamples.java ]]
then
   echo "The Testlistexamples file is been copy"
else
   echo "The Testlistexamples file is not been copy"
   exit 1
fi

cpath=".:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar"

set +e
javac -cp $cpath *.java


if [[ $? -eq 0 ]]
then
  echo "compiled"
else
  echo "didn't compiled"
  exit 1
fi

java -cp $cpath org.junit.runner.JUnitCore TestListExamples > out.txt

if [[ $? -eq 0 ]]
then
  grep "OK" out.txt
  exit 0
else
  grep "Tests run:" out.txt
  exit 1
fi
```

# Example

![Image](Lab9pic\Runing1.PNG)

![Image](Lab9pic\runing2.PNG)

![Image](Lab9pic\runign3.PNG)

# Explanation of example

## https://github.com/ucsd-cse15l-f22/list-methods-lab3

set -e doesn't have standard output or standard error; return code 0

rm -rf student-submission, return code 0

git clone $1 student-submission
standard output is "cloning into 'student..."
no standard error here; return 0

echo "successfully copy"
standard output is "successfully copy"
return 0

cd student-submission
no std output or std err
return 0

if [[ -e ListExamples.java ]]
is true, return 0

echo "The file exist"
std output is "The file exist"
return 0;

```
else
    echo "The file not found"
    echo "Maybe Wrong File Name"
    exit 1
fi
```
Doesn't run, because it's in if else branch

cd ../
redirected to upper directory, no std output or err; return 0

cp -rf lib student-submission
copy
cp -f TestListExamples.java student-submission