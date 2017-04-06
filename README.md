# PlanetEarth.py
class Continent:
    continentcount = 0
    name = ""
    def __init__(self, name):
        print("Calling Continent constructor")
        self.name= name
        Continent.continentcount += 1
    def getval(self):
        print(self.name)
    @classmethod
    def howmany(cls):
        print("Continent count: ", cls.continentcount)

class Country(Continent):
     Name = 0
     countrycount = 0
     population = 0
     capital = 0
     nationallanguage = 0
     currency = 0
     president = 0
           
     def __init__(self):
         print("Calling Country constructor")

     def setval(self, name, population, capital, nationallanguage, currency, president):
         self.name = name
         self.population = population
         self.capital = capital
         self.nationallanguage = nationallanguage
         self.currency = currency
         self.president = president
         Country.countrycount += 1
     def getval(self):
         print (self.name, "Population: ", self.population,"\n", "Capital: ", self.capital,"National Language:", self.nationallanguage, "Currency:", self.currency,"President:", self.president)
     @classmethod
     def howmany(cls):
         print("Country count is: ", cls.countrycount)

p1 = Continent("Europe")                            # p1.setval("Europe")
p1.getval()
Continent.howmany()
print("\n\n")
s1= Country()
s1.setval("England\n",52010000,"London\n","English\n","BPD\n","Theresa May")
s2= Country()
s2.setval("France\n", 66030000,"Paris\n", "French\n","EUR\n","Francois Hollande")
s3= Country()
s3.setval("Germany\n", 80620000,"Berlin\n", "German\n","EUR\n","Angela Merkel")
s1.getval()
s2.getval()
s3.getval()
Country.howmany()
Continent.howmany()
print("\n\n")

p2 = Continent("Africa")                            # p2.setval("Africa")
p2.getval()
Continent.howmany()
print("\n\n")
s4= Country()
s4.setval("South Africa\n", 52980000,"Pretoria\n","English\n","ZAR\n","Jacob Zuma")
s5= Country()
s5.setval("Nigeria\n", 188462000,"Abuja\n","English\n","NGN\n","Muhammadu Buhari")
s6= Country()
s6.setval("Zimbabwe\n", 14150000,"Harare\n","English\n","USD\n","Robert Mugabe")
s4.getval()
s5.getval()
s6.getval()
Country.howmany()
Continent.howmany()
print("\n\n")

p3 = Continent("Asia")                            # p3.setval("Asia")
p3.getval()
Continent.howmany()
print("\n\n")
s7= Country()
s7.setval("China\n", 1373500000,"Beijing\n","Chinese\n","CNY\n","Xi Jinping")
s8= Country()
s8.setval("India\n", 1310069000,"New Delhi\n","Hindi\n","INR\n","Pranab Mukherjee")
s9= Country()
s9.setval("Pakistan\n", 201990000,"Islamabad\n","Urdu\n","PKR\n","Mamnoon Hussain")
s7.getval()
s8.getval()
s9.getval()
Country.howmany()
Continent.howmany()
print("\n\n")

p4 = Continent("North America")                            # p3.setval("Asia")
p4.getval()
Continent.howmany()
print("\n\n")
s10= Country()
s10.setval("USA\n", 333500000,"Washington DC\n","English\n","USD\n","D. Trump")
s11= Country()
s11.setval("Mexico\n", 120069000,"Mexico City\n","Spanish\n","MXN\n","Enrique Pena Nieto")
s12= Country()
s12.setval("Canada\n", 35190000,"Ottowa\n","English\n","CAD\n","Justin Trudeau")
s10.getval()
s11.getval()
s12.getval()
Country.howmany()
Continent.howmany()
print("\n\n")

