##  Implement Tower of Hanoi Using Recursion

## Aim:
To write a Python program that solves the Tower of Hanoi problem recursively and displays all the moves made to shift disks from source peg to destination peg.

## Procedure:

1.Get the number of disks from the user.

2.Define a recursive function tower_of_hanoi(n, source, auxiliary, destination):

  If n == 1, move the disk directly from source to destination.

  Otherwise, move n-1 disks from source to auxiliary using destination as temporary.

  Move the remaining disk to the destination.

  Move the n-1 disks from auxiliary to destination using source as temporary.

3.Call the recursive function with pegs named A (source), B (auxiliary), and C (destination).

4.Display each move.
## Program:
```python
def TowerOfHanoi(n , source, destination, auxiliary):
	
	if(n>0):
	    TowerOfHanoi(n-1, source, auxiliary, destination)
	    print ("Move disk from",source,"to",destination)
	    TowerOfHanoi(n-1, auxiliary, destination, source)

n=int(input())		
print("No. of disks =",n)

```

## Output:
![image](https://github.com/user-attachments/assets/e513a805-1a25-47a2-b27a-372b4204eac4)

## Result:
The program displays all the steps to move the given number of disks from peg A to peg C following the rules of the Tower of Hanoi puzzle using a recursive approach.
