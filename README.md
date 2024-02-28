# sum-of-max_even-and-max_odd-
#sum of odd and even in a list
# approach-1
n=int(input())
a=list(map(int,input().split()))
r=0
k=0
for i in range(n):
  if a[i]%2==0 and a[i]>r:
    r=r+a[i]
  elif a[i]>k:
    k=k+a[i]
print(r)
print(k)
print(r,k)
print(r+k)

#approach-2
n=int(input())
a=list(map(int,input().split()))
r=0
k=0
for i in a:
  if i%2==0 and i>r:
    r=r+i
  elif i>k:
    k=k+i
print(r)
print(k)
print(r+k)

#approach-3
n=int(input())
a=list(map(int,input().split()))
r=[]
k=[]
for i in range(n):
  if a[i]%2==0 :
    r.append(a[i])
  else:
    k.append(a[i])
print(max(r)+max(k))

#approach-4
n=int(input())
a=list(map(int,input().split()))
r=[]
k=[]
for i in a:
  if i%2==0:
    r.append(i)
  else:
    k.append(i)
print(max(r)+max(k))
print(max(k))
print(max(r))
