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
 
## Sources Used:


1) Used ChatGPT to find the commands.
