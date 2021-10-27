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

  ```
