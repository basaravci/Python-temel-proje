#1.soru cevabı--------------------
a=[[1,'a',['cat'],2],[[[3]],'dog'],4,5]

b=[]

def flatten(l):
      
    for i in l:
        if isinstance(i,list):
            flatten(i)
        else:
            b.append(i)
    return b
print(flatten(a))

#2.soru cevabı--------------------

c=[[1, 2], [3, 4], [5, 6, 7]]

d=[]

def rev(x):

    for i in x:
        d.append(list(reversed(i)))
    return list(d.__reversed__())       
print((rev(c)))
