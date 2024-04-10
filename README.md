print("Welcome to my family tree")
#creating the parent class
class FamilyMember:
    def __init__(self,fname,lname):
        self.firstname = fname
        self.lastname = lname
#function that will print the name of memeber
    def printname(self):
        print(self.firstname, self.lastname )
# creating HouseSpain subclass that will have all the spanish members
class HouseSpain(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

    def __init__(self, fname, lname, location):
       FamilyMember.__init__(self, fname, lname)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname)
       self.familytext = location
    
    def printinfo(self):
             print(self.firstname, self.lastname, "is of house" + self.familytext)

x = HouseSpain("Rachel", "Turner", "spain")
x.printinfo()
y = HouseSpain("Maya", "Guyon Turner", "spain")
y.printinfo()
z = HouseSpain("Ela", "Guyon Turner", "spain")
z.printinfo()
t = HouseSpain("Mathieu", "Guyon", "spain")
t.printinfo()

class HouseAustralia(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

    def __init__(self, fname, lname, location):
       FamilyMember.__init__(self, fname, lname)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname)
       self.familytext = location
    
    def printinfo(self):
             print(self.firstname, self.lastname, "is of house" + self.familytext)

x = HouseAustralia("Paul", "Turner", "australia")
x.printinfo()
y = HouseAustralia("Mary", "Turner", "australia")
y.printinfo()
z = HouseAustralia("Ben", "Turner", "australia")
z.printinfo()
t = HouseAustralia("James", "Turner", "australia")
t.printinfo()

class HouseUk(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

    def __init__(self, fname, lname, location):
       FamilyMember.__init__(self, fname, lname)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname)
       self.familytext = location
    
    def printinfo(self):
             print(self.firstname, self.lastname, "is of house" + self.familytext)

x = HouseUk("Daniel", "Turner", "uk")
x.printinfo()
y = HouseUk("Scarlet", "Turner", "uk")
y.printinfo()
z = HouseUk("India", "Turner", "uk")
z.printinfo()
t = HouseUk("Thomas", "Guyon", "uk")
t.printinfo()

class HouseFrance(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

    def __init__(self, fname, lname, location):
       FamilyMember.__init__(self, fname, lname)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname)
       self.familytext = location
    
    def printinfo(self):
             print(self.firstname, self.lastname, "is of house" + self.familytext)

x = HouseFrance("Nicole", "Guyon", "france")
x.printinfo()
y = HouseFrance("Anne", "Guyon", "france")
y.printinfo()
z = HouseFrance("Benoit", "Guyon", "france")
z.printinfo()
t = HouseFrance("Laura", "Guyon", "france")
t.printinfo()
