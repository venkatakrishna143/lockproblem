# lockproblem

n=int(input())
l=[]
for i in range(n):
        l.append(int(input()))
def fun(sum,index,l):
        if(index==len(l)):
                if(sum==0 or sum==360):
                        return True
                return 
        return fun(sum-l[index],index+1,l) or fun(sum+l[index],index+1,l)
if(fun(0,0,l)):
        print("YES")
else:
        print("NO")
