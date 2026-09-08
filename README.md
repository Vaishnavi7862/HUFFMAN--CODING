# Huffman-Coding
## Aim
To implement Huffman coding to compress the data using Python.

## Software Required
Anaconda - Python 3.7
## Step1:
Get the input string.

## Step2:
Create tree nodes.

## Step3:
Main function to implement huffman coding.

## Step4:
calculate frequency of occurence.

## Step5:
print the characters and its huffmancode.

## Program:
```
import math

p = [0.4, 0.3, 0.15, 0.10, 0.05]
code = ['1', '01', '001', '0000', '0001']

# Average code length
L = sum(p[i] * len(code[i]) for i in range(5))

# Entropy
H = sum(x * math.log2(1/x) for x in p)

# Coding efficiency
eff = H / L

# Redundancy
R = 1 - eff

print("Huffman Codes:")
for i in range(5):
    print("a", i+1, "=", code[i])

print("Average Code Length =", L)
print("Entropy =", round(H, 4))
print("Coding Efficiency =", round(eff, 2))
print("Redundancy =", round(R, 2))
```
## Output:
<img width="265" height="217" alt="image" src="https://github.com/user-attachments/assets/09a6a9a8-eed5-4bce-9f04-f9a4ac54f9ec" />

## Result:
Thus the huffman coding was implemented to compress the data using python programming.
