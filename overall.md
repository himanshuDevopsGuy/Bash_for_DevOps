# Loops ➿

## Why Loops

- To perform a repetitive task for achieving the desired target we make use of loops.
> Benefits
  - Saves Time
  - Reduces the probability of errors 

### Types of Loops in Bash 

- Until
- While
- For


## While Loop 

### Basic Syntax 🔣
```
#!/bin/bash
while[condition]
do
  command 1
  command n
done
```

## Until Loop

## Basic Syntax
```
#!/bin/bash
until [condition];
do
  command 1
  command n
done

```

### WHILE VS UNTIL LOOP 🤔

- **While Loop** executes the block of code (enclosed in do...done) **when the condition is true** and **keeps executing that till the condition becomes false.** Once the condition becomes false, the while loop is terminated.

- **Until Loop** executes the block of code (enclosed in do...done) **when the condition is false** and **keep executing that till the condition becomes true.** Once the condition becomes true, the until loop is terminated.


# Getting started with For loops ➰

## Basic syntax

- 
```
  #! /bin/bash 

  for i in num1 num2 numn
  do
    Command 1
    Command n
  done
```

- 
```
#! /bin/bash 
for i in {Begin_number..End_number..increment_number}
do
  Command 1 
  Command n
done
```

## For with Numeric Values ➿

- Example 1
  - for_numeric.sh 
    - ```
        #! /bin/bash 
        # i --> you can consider as variable

        for i in 1 2 3 4 5 6 7 8 9 10
        do
          echo "HelloCount--"$i
          echo "any command--"$i
        done
        ```
### bappan's issue
```
trainers = (mohan, bhupender, pankaj, Prakash, Vikas, Himanshu)
echo ${trainers[@]}
echo ${!trainers[@]}
for i in ${!trainers[@]}
do
  echo "Trainer is ${trainer[$i]} and its index is $i"
done  
```


     - Now suppose you just want to give a range `{begin..end}`
         - ``` 
            ## it will starts for 1 and end to 10 
            ## the syntax basically represents {BeginNumber..EndNumber}

            for i in {1..10}
            do
              echo "countTime--"$i
            done
            ```

      - Range with increment `{begin..end..increment}`
        - ```
            ## Now lets suppose you want to increment the variable count for eg: expected output to come like :
            ## countTime--1
            ## countTime--3
            ## the series will be like 1,3,5,7,9

            ## the syntax is having one extra argument which is increment value {begin..end..increment}
            for i in {1..10..2}
            do
              echo "Odd-Series-Count--"$i
            done

            ```
## Infinite Loops ➿

- ```
    #! /bin/bash

    for (( ; ; ))
    do
      echo "HI"
    done
  ```
## for with expressions ➿

- ```
  for((i=1;i<=5;i++))
  do
    echo $i
  done
  ```



## while vs for when to use and when not to 🤔

- If you know prior to the loop how many repetitions you are going to need, such as iterating a countable number of static files to process, you should use a for loop. That is what for loops are good at doing. If you are unsure, and the loop may be different based on what happens during processing, such as some sort of iterative aggregation algorithm that fills an accumulator to a certain value, or a search algorithm that will drop out of the loop when it finds the value that it is looking for, then use a while loop.

## Seq Command

```
seq Starting_num increment_num ending_num
```
- Using with loops
```
#!/bin/bash
for i in $(seq 1 2 20)
do
   echo "Welcome $i times"
done

```

## Patterns
- Basic
```
12345
12345
12345
12345
12345
```
- Design 1
```
1
12
123
1234
12345
```
