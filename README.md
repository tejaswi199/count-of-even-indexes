#Approach-1
s=(input())
c=0
for i in range(len(s)):
  if i%2==0:
    c=c+1 
print(c)

#Approach-2
s=input()
x=s[::2]
print(len(x))

#Approach-3
s=input()
x=[]
for i in range(len(s)):
  if i%2==0:
    x.append(s[i])
y=[]
for i in range(len(s)):
  if i%2!=0:
    y.append(s[i])
x.extend(y)
print(*x,sep="")

#Approach-4
s=input()
x=""
y=""
for i in range(len(s)):
  if i%2==0:
    x=x+s[i]
for i in range(len(s)):
  if i%2==0:
    y=y+s[i]
print(x+y)

#Approach-5
s=input()
x=s[::2]
y=s[1::2]
print(x+y)

