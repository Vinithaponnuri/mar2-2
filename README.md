PROGRAMME:
A=[]
m=int(input('enter no of rows: '))
n=int(input('enter no of columns: '))
for i in range(m):
    row=[]
    for j in range(n):
        k=int(input())
        row.append(k)
    A.append(row)
print(A)
B=[]
m=int(input('enter no of rows: '))
n=int(input('enter no of columns: '))
for i in range(m):
    row=[]
    for j in range(n):
        k=int(input())
        row.append(k)
    B.append(row)
print(B)
result=[[0,0],[0,0]]
for i in range(m):
    for j in range(n):
        result[i][j]=[A[i][j]*B[i][j]]
print('resultant matrix is: ',end=' ')
for i in range(m):
    for j in range(n):
        print(result[i][j],end=' ')
    print()
    OUTPUT:
    enter no of rows: 2
enter no of columns: 2
1
2
3
4
[[1, 2], [3, 4]]
enter no of rows: 2
enter no of columns: 2
1
2
3
4
[[1, 2], [3, 4]]
resultant matrix is:  [1] [4] 
[9] [16] 

OR

A=[]
m=int(input('enter no of rows: '))
n=int(input('enter no of columns: '))
for i in range(m):
    row=[]
    for j in range(n):
        k=int(input())
        row.append(k)
    A.append(row)
print(A)
for i in range(m):
    for j in range(n):
        print(A[i][j],end=' ')
    print()
for i in range(m):
    for j in range(n):
        print(A[j][i],end=' ')
    print()
trace=0
for i in range(m):
    for j in range(n):
        trace=trace+A[i][j]
        print(trace,end=' ')
    print()
    OUTPUT:
    enter no of rows: 2
enter no of columns: 2
1
2
3
4
[[1, 2], [3, 4]]
1 2 
3 4 
1 3 
2 4 
1 3 
6 10 

