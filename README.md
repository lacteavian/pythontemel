# pythontemel
originallist=[[1,'a',['cat'],2],[[[3]],'dog'],4,5]
newlist=[]
def flattenlist(x):
    for i in x:
        if type(i) == list:
            flattenlist(i)
        else:
            newlist.append(i)
    return newlist
print(flattenlist(originallist))

list1=[[1, 2], [3, 4], [5, 6, 7]]
list2=[]
def reverselist(y):
    for i in sorted(y,reverse=True):
        list2.append(sorted(i, reverse=True))
    return print(list2)
reverselist(list1)
