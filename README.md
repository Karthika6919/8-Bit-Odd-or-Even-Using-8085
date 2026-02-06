# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:
```
LDA 4200H
ANI 01H
JZ L1
MVI A, 01H
JMP L2
L1: MVI A,02H
L2: STA 4201H
HLT
```
## Output:

<img width="1818" height="785" alt="Screenshot 2026-02-06 135043" src="https://github.com/user-attachments/assets/e80f7d86-cd51-4677-b305-cd7b9351f498" />
<img width="1818" height="772" alt="Screenshot 2026-02-06 135157" src="https://github.com/user-attachments/assets/90d66fe4-177f-4b0d-a394-476f723a1320" />
<img width="531" height="882" alt="Screenshot 2026-02-06 141704" src="https://github.com/user-attachments/assets/934990f5-d7a1-4be3-98c4-dafa75278652" />

## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

