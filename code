import pandas as pd
import matplotlib.pyplot as plt

# Museum ID,Museum Name,Legal Name,Alternate Name,Museum Type,Institution Name,Street Address (Administrative Location),City (Administrative Location),State (Administrative Location),Zip Code (Administrative Location),Street Address (Physical Location),City (Physical Location),State (Physical Location),Zip Code (Physical Location),Phone Number,Latitude,Longitude,Locale Code (NCES),County Code (FIPS),State Code (FIPS),Region Code (AAM),Employer ID Number,Tax Period,Income,Revenue
#data




df = pd.read_csv (r"museums_abridged.csv")
pd.set_option("display.max_columns" , None)



print("This presentation is about wich museam is most succsessfull in indiana.")
print("------------------------------------------------------------------------")
print()
print()
print()


print("The muesum's names and Ids and types.")
print("------------------------------------------------------------------------")
filterd_table = df[["Museum Name" , "Museum ID" , "Museum Type"]]
print(filterd_table)
print("------------------------------------------------------------------------")

print()
print()

print("The musuems Tax Rate and income and Revenue")
print("------------------------------------------------------")
table = df[["Museum Name" , "Income" , "Tax Period" , "Revenue"]]
print(table)
print("------------------------------------------------------")


print()
print()

print("Who has the most and least amount of income?")
print("----------------------------------------------------")
print("Most Income")
print()
Income1 = df[["Museum Name" ,"Income" , "Tax Period" , "Revenue"]].max()
print(Income1)
print()
print()
print("Least Income")
Income2 = df[["Museum Name" , "Income" , "Tax Period" , "Revenue"]].min()
print(Income2)
print()


print("----------------------------------------------------")
print()
print()
print("Diffrent persentiges of income.")
print("------------------------------------------------------")

s = df[["Museum Name" ,"Income" , "Tax Period" , "Revenue"]].describe()
print(s)
print("----------------------------------------------------")

print()
print()

def avrege():
    print("Range of the income")
    print("--------------------------------------------------")
    max1 = df[["Income" , "Tax Period" , "Revenue" ]].max()
    min1 = df[["Income" , "Tax Period" , "Revenue"]].min()
    print(max1 - min1)
    print("--------------------------------------------------")

avrege()

print()
print()

print("box plot of income between the top banks")
print("---------------------------------------------------------")
my_data = pd.Series([2908175692.0 , 201006.0  ], 
index = ["ZION NATURE CENTER total income" , "44TH INDIANA CIVIL WAR HISTORICAL ASSOCIATION total income" ])
plt.boxplot(my_data)
plt.show()
print("---------------------------------------------------------")
print()
print()
print("Awnser")
print("--------------------------------------------------")
print("The most sucsessful museum was ZION NATURE with a total income of 2908175692.0 dollars out of all the museams in indiana. ")
