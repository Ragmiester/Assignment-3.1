# Assignment-3.1
a=input("enter the no.s to be reduced and filtered: ")
b=a.split(",")
g=[int(n) for n in b]
def my_reduce(d):
    c=d[0]
    for i in range(len(d)-1):
        c += d[i+1]
    return c
def my_filter(d):
    c=[]
    for i in d:
        if i%2==0:
            c.append(i)
    return c
print("the reduced no. is: ",my_reduce(g))
print("the even filtered no.s are: ",my_filter(g))
