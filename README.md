'''
Problem Statement 1:
Write a Python Program(with class concepts) to find the area of the triangle using the
below formula.
area = (s*(s-a)*(s-b)*(s-c)) ** 0.5
Function to take the length of the sides of triangle from user should be defined in the
parent class and function to calculate the area should be defined in subclass.

Problem Statement 2:
Write a function filter_long_words() that takes a list of words and an integer n and returns
the list of words that are longer than n.
'''


# 2.4.1
class tarea:    
    def __init__(self):
        self.a = 0
        self.b = 0
        self.c = 0
    def insert_sides(self):
        self.a = int(input("insert side a value : "))
        self.b = int(input("insert side b value : "))
        self.c = int(input("insert side c value : "))
 
class sarea(tarea):
    def __init__(self):
        tarea.__init__(self)
    def area(self):
        s = (self.a + self.b + self.c)/2
        return(s * (s-self.a) * (s-self.b) * (s-self.c)) ** 0.5
        
        
xyz = sarea()
xyz.insert_sides()
print(xyz.area())


#2.4.2
l7=["abc","pqrst","uvwxyzasawq","lmnop","uvwxyz"]
len1=5
for p in l7:
    x=len(p)
    if x>len1:
        print(p)
