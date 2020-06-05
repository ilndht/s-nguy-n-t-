# s-nguy-n-t-
import math
n = int(input(" n :"))
a = math.sqrt(n)
x = math.floor(a)                   # x= phần nguyên của căn n 
A= range ( 1,n)
A= [True for m in range(1,n)]
for i in range (2,x+1) :
    for j in range (2*i,n,i):
                A[j-1]= False
h= len([k for k in A if k == True])
print(h-1)

