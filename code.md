# Convert binary numbers into decimal numbers

def convert(binary_number):
 length=len(binary_number)-1
 decimal_number=0
 for digit in binary_number:
  if digit == "1":
   decimal_number += 2**(length - binary_number.index(digit))
  length -=1
 print(decimal_number)
 print("\n")

while 1==1:
 binary_number=input("Enter a binary number: ")
 error= False
 for digit in binary_number:
  if not(digit=="0" or digit=="1"):
   error = True
 if error == True:
  print("ERROR")
  print("\n")
 else:
  convert(binary_number)
