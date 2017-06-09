import sys
import math

# Auto-generated code below aims at helping you parse
# the standard input according to the problem statement.

n = int(input())  # the number of temperatures to analyse
temps = [ int(i) for i in input().split()]  # the n temperatures expressed as integers ranging from -273 to 5526

# Write an action using print
# To debug: print("Debug messages...", file=sys.stderr)

    
min=5527
for i in temps:
    if abs(i)<abs(min) : min=i
    elif i==-min : min=abs(min)
    
if min == 5527:
    r = 0
else:
    r=min
    

print(r)
