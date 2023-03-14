# Using the ```grep``` command

Five commands being explored here:
#### 1) grep -r pattern dir: Without regard to case, this command looks for lines in the provided file(s) that have the specified pattern.
#### 2) grep -i pattern file: This command searches for lines in the specified file(s) that contain the given pattern, ignoring case sensitivity.
#### 3) grep -v pattern file: This command looks for lines that don't match the supplied pattern in the specified file(s).
#### 4) grep -c pattern file: The number of lines in the specified file(s) that match the specified pattern is counted by this command.
#### 5) grep -n pattern file: The line numbers of lines in the provided file(s) that contain the specified pattern are displayed by this command.

## grep -r pattern dir
Current working directory: Abernathy
       
Using the command
       
       
```
grep -r Misalignment .
```


       
Output: 
       
```
./ch8.txt:Simpler spreading machines have no on-board computer, but they do unroll the bolt of cloth 
“unstressed” and properly aligned with the edge of the ply below. However spreading is done, 
it is important for the plies to lie directly on top of each other. Misalignment of the edges can ruin 
many pattern pieces and the final garments for which they were intended. Once a ply is laid down, it is 
almost impossible to shift it because of the friction between the plies. With simple spreading machines,
the operator must look for fabric defect indicators placed in the selvage by the textile manufacturer.
```

Second example:
Using the command
```
grep -r friction .
```

Output
```
./ch8.txt:Spreading cloth out on a table in a way that leaves it flat but unstretched, without tension 
in the cloth, is more difficult than one would think. To get the cloth flat, without mechanical help, 
two workers could hold the cloth by both ends and stretch it out flat, then release just one end. But 
the friction between the table and the cloth will leave this layer (“ply”) of cloth stretched; just how 
much will depend on the amount of friction between the two. Putting another ply on top the same way creates 
an additional problem. The friction between the second ply and the first can create a wrinkle in the 
first ply. When plies of cloth are piled high—a foot or more is not unusual—there are often wrinkles in 
the plies after they are cut. This is especially true for knit goods, which are easily stretched and adhere 
well to neighboring plies in a stack of cloth.
./ch8.txt:Simpler spreading machines have no on-board computer, but they do unroll the bolt of cloth 
“unstressed” and properly aligned with the edge of the ply below. However spreading is done, it is important 
for the plies to lie directly on top of each other. Misalignment of the edges can ruin many pattern pieces 
and the final garments for which they were intended. Once a ply is laid down, it is almost impossible to 
shift it because of the friction between the plies. With simple spreading machines, the operator must look 
for fabric defect indicators placed in the selvage by the textile manufacturer.
```



The command finds the file in the directory with the word "Misalignment".
## grep -i pattern dir
Current working directory: Abernathy
 Using the command:
 
 ```
 grep -i misalignment ./ch8.txt
 ```
 
 Output:
 ```
 Simpler spreading machines have no on-board computer, but they do unroll the bolt of cloth “unstressed” 
 and properly aligned with the edge of the ply below. However spreading is done, it is important for the 
 plies to lie directly on top of each other. Misalignment of the edges can ruin many pattern pieces and the 
 final garments for which they were intended. Once a ply is laid down, it is almost impossible to shift it 
 because of the friction between the plies. With simple spreading machines, the operator must look for fabric
 defect indicators placed in the selvage by the textile manufacturer.
 ```
 The command, as seen, is not case sensitive.
 
Second example:
Using the command
```
grep -i Friction ./ch8.txt
```

Output
```
Spreading cloth out on a table in a way that leaves it flat but unstretched, without tension in the cloth, 
is more difficult than one would think. To get the cloth flat, without mechanical help, two workers could 
hold the cloth by both ends and stretch it out flat, then release just one end. But the friction between 
the table and the cloth will leave this layer (“ply”) of cloth stretched; just how much will depend on the 
amount of friction between the two. Putting another ply on top the same way creates an additional problem. 
The friction between the second ply and the first can create a wrinkle in the first ply. When plies of cloth 
are piled high—a foot or more is not unusual—there are often wrinkles in the plies after they are cut. This 
is especially true for knit goods, which are easily stretched and adhere well to neighboring plies in a stack 
of cloth.
Simpler spreading machines have no on-board computer, but they do unroll the bolt of cloth “unstressed” and 
properly aligned with the edge of the ply below. However spreading is done, it is important for the plies to 
lie directly on top of each other. Misalignment of the edges can ruin many pattern pieces and the final garments
for which they were intended. Once a ply is laid down, it is almost impossible to shift it because of the friction 
between the plies. With simple spreading machines, the operator must look for fabric defect indicators placed 
in the selvage by the textile manufacturer.
```

## grep -v pattern dir
 Current working directory: Abernathy
 
 Using the command:
 
 ```
 grep -v of ./ch8.txt
 ```
 
 Output:
 ```
The First Step: Apparel Design and Patterns
Preassembly: Marker-Making
Preassembly: Spreading
Preassembly: The Cutting Room
Bundling the Parts
Mass Customization
From Preassembly to Assembly
 ```
Finds all the lines that do not contain the word "of"
 
Second example:
Using the command
```
grep -v or ./ch8.txt
```

Output
```
The First Step: Apparel Design and Patterns
Note that this entire design sequence can take as little as part of a day, yielding a sample garment 
hung on a mannequin. Again, the time it takes managers to reach a decision is what determines the length 
of this process. However, it may take months 
to produce a sample garment in a desired fabric simply because that fabric takes months to make.
Preassembly: Marker-Making
Preassembly: Spreading
Preassembly: The Cutting Room
Bundling the Parts
Mass Customization
From Preassembly to Assembly
```
 

 
 ## grep -c pattern file
 Current working directory: Abernathy
 
 Using the command:
 
 ```
 grep -c of ./ch8.txt
 ```
 
 Output:
 ```
 66
 ```
 66 lines that have the word of.

Second example:
Using the command
```
grep -c friction ./ch8.txt
```

Output
```
2
```
 
 ## grep -n 
 
 Current Working directory 
 
 Using the command
 
 ```
 grep -n Misalignment ./ch8.txt
 ```
 
 Output:
```
40:Simpler spreading machines have no on-board computer, but they do unroll the bolt of cloth 
“unstressed” and properly aligned with the edge of the ply below. However spreading is done, 
it is important for the plies to lie directly on top of each other. Misalignment of the edges 
can ruin many pattern pieces and the final garments for which they were intended. Once a ply 
is laid down, it is almost impossible to shift it because of the friction between the plies. 
With simple spreading machines, the operator must look for fabric defect indicators placed in 
the selvage by the textile manufacturer.
```


Second example:
Using the command
```
grep -n wrinkle ./ch8.txt
```

Output
```
37:Spreading cloth out on a table in a way that leaves it flat but unstretched, without tension in
the cloth, is more difficult than one would think. To get the cloth flat, without mechanical help, 
two workers could hold the cloth by both ends and stretch it out flat, then release just one end. 
But the friction between the table and the cloth will leave this layer (“ply”) of cloth stretched; 
just how much will depend on the amount of friction between the two. Putting another ply on top the 
same way creates an additional problem. The friction between the second ply and the first can create 
a wrinkle in the first ply. When plies of cloth are piled high—a foot or more is not unusual—there
are often wrinkles in the plies after they are cut. This is especially true for knit goods, which 
are easily stretched and adhere well to neighboring plies in a stack of cloth.
```
 
## Sources Used:


1) Used ChatGPT to find and understand the commands.
