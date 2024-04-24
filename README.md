print("Welcome to my family tree")
#creating the parent class
class FamilyMember:
    def __init__(self,fname,lname,generation,side):
        self.firstname = fname
        self.lastname = lname
        self.generation = generation
        self.side = side 

#function that will print the name of memeber
    def printname(self):
        print(self.firstname, self.lastname, self.generation, self.side)
# creating HouseSpain subclass that will have all the spanish members
class HouseSpain(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

    def __init__(self, fname, lname, generation, side, location):
       FamilyMember.__init__(self, fname, lname, generation, side)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname, generation, side)
       self.familytext = location
    
    

familyspainList = []
familyspainList.append(HouseSpain("Rachel", "Turner", 2, "mum", "Spain"))
familyspainList.append(HouseSpain("Mathieu", "Guyon", 2, "dad","Spain"))
familyspainList.append(HouseSpain("Maya", "Turner", 3, "both", "Spain"))
familyspainList.append(HouseSpain("Ela", "Turner", 3, "both", "Spain"))

for HouseSpain in familyspainList:
    print("name : {}, lastname : {}, generation : {}, side : {}, location : {}".format(HouseSpain.firstname, HouseSpain.lastname, HouseSpain.generation, HouseSpain.side, HouseSpain.familytext))

class HouseAustralia(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

   def __init__(self, fname, lname, generation, side, location):
       FamilyMember.__init__(self, fname, lname, generation, side)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname, generation, side)
       self.familytext = location
    


familyaustraliaList = []
familyaustraliaList.append(HouseAustralia("Ben", "Turner", 3, "mum", "Australia"))
familyaustraliaList.append(HouseAustralia("Mary", "Turner", 3, "mum", "Australia"))
familyaustraliaList.append(HouseAustralia("Paul", "Turner",2, "mum", "Australia"))
familyaustraliaList.append(HouseAustralia("James", "Turner", 2 , "mum", "Australia"))

for HouseAustralia in familyaustraliaList:
     print("name : {}, lastname : {}, generation : {}, side : {}, location : {}".format(HouseAustralia.firstname, HouseAustralia.lastname, HouseAustralia.generation, HouseAustralia.side, HouseAustralia.familytext))

class HouseUk(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

     def __init__(self, fname, lname, generation, side, location):
       FamilyMember.__init__(self, fname, lname, generation, side)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname, generation, side)
       self.familytext = location
   

familyukList = []
familyukList.append(HouseUk("Daniel","Turner", 2, "mum" ,  "Uk"))
familyukList.append(HouseUk("Scarlet", "Turner", 3, "mum" , "Uk"))
familyukList.append(HouseUk("India", "Turner", 3, "mum" , "Uk"))
familyukList.append(HouseUk("Thomas", "Guyon", 3, "dad" , "Uk"))

for HouseUk in familyukList:
     print("name : {}, lastname : {}, generation : {}, side : {}, location : {}".format(HouseUk.firstname, HouseUk.lastname, HouseUk.generation, HouseUk.side, HouseUk.familytext))

class HouseFrance(FamilyMember):
    # now subclass has its own init funccion (this is callet "overriding")

     def __init__(self, fname, lname, generation, side, location):
       FamilyMember.__init__(self, fname, lname, generation, side)
       # Super key word will make the child inherit everything from parent
       super().__init__(fname, lname, generation, side)
       self.familytext = location
    
    

familyfranceList = []
familyfranceList.append(HouseFrance("Nicole", "Guyon", 1, "dad" ,  "France"))
familyfranceList.append(HouseFrance("Benoit", "Guyon",  2, "dad" , "France"))
familyfranceList.append(HouseFrance("Anne", "Guyon",  2, "dad" , "France"))
familyfranceList.append(HouseFrance("Laura", "Guyon", 3, "dad" ,  "France"))

for HouseFrance in familyfranceList:
     print("name : {}, lastname : {}, generation : {}, side : {}, location : {}".format(HouseFrance.firstname, HouseFrance.lastname, HouseFrance.generation, HouseSpain.side, HouseFrance.familytext))



