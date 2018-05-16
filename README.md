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
