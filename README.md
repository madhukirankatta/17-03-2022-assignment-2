# 17-03-2022-assignment-2
#program to print the given password is valid or not.
#password should contain at least 1 upper,lower,symbol and digit.
s=input()#taking password
l1=list(s)
l=0
u=0
d=0
s=0
for i in l1:
    if(i.islower()):
        l=l+1
    elif(i.isupper()):
        u=u+1
    elif(i.isdigit()):
        d=d+1
    else:
        s=s+1
if l>=1 and u>=1 and d>=1 and s>=1:
    print("The password is valid")
else:
    print("the password is not valid")
if l<=0 or u<=0 or d<=0 or s<=0:
    print("password should contain at least 1 uppercase,lowercase,symbol and digit")
