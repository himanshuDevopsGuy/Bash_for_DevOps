# Getting started with patterns with loops: 🐉


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
- Design 2 (Reversing j values)
```
5
54
543
5432
54321
```
- Design 3 
```
    5
   45
  345
 2345
12345
```
```
#!/bin/bash



for((i=1;i<=5;i++))
do
        for((j=1;j<=5;j++))
        do
                if [ 5 -le $(($i+$j-1))  ]
                then
                        echo -ne "$j"
                else
                        echo -ne " "
                fi
        done
        echo ""
done

```
- Design 4
```
54321
 4321
  321
   21
    1
```

```
for((i=1;i<=5;i++))
do
        for((j=5;j>=5;j--))
        do
                if [ 5 -le $(($i+$j-1))  ]
                then
                        echo -ne "$j"
                else
                        echo -ne " "
                fi
        done
        echo ""
done
```
- Design 
```
    1
   22
  333
 4444
55555

```
```
#!/bin/bash



for((i=1;i<=5;i++))
do
        for((j=1;j<=5;j++))
        do
                if [ 5 -le $(($i+$j-1))  ]
                then
                        echo -ne "$i"
                else
                        echo -ne " "
                fi
        done
        echo ""
done

```
