# pgm-cm1.py
count=0
n int(input())
for i in range(1,n):
    for j in range(1,n):
        for k in range(1,n):
            if(i+j+k)==n:
                if((i==j and i<k)or(j==k and j<i)or(i==k and i<j)or(i!=k and i!=j and j!=k)):
                    count+=1 
                    if(i+j+k)>n:
                        break
print(count)
