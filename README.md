# balance-calculator-project
Name: Alex Gordon
Date Due: 12/21/2017
Class: 12 B
Goal: The goal of this project is to create a calculator that calculates both the interest rate of a bank account and displays the total balance for n years with compounded interest.
Code for the calculator
interestRate=float(input("what is the interestRate"))/100+1
startingPrice=float(input("what is the startingPrice"))
numberofYears=int(input("what is the numberofYears"))+1
for yearNumber in range(numberofYears):
  print(startingPrice*interestRate**yearNumber)
  
 
 Side note: It automatically bolded when I put two multiplication symbols (2 of *). Didn't intend for that to be bolded in the code, but wasn't sure how to undo the bolding.
 
 Math to solve problem: 
 If interestRate is 15%, startingPrice is $25, and numberofYears is 5 years.
 It fist can be said that the price for the 0th year is $25 because no interest in being added initally.
 Next, do interestRate/100 (15%/100) to get a decimal. This decimal is .15. Then add 1 to this value to make sure the resulting number goes up and not down > .15+1=1.15. This was (interestRate)/100+1.
 Next to calculate the balance after 1 year one must do (startingPrice*intrestRate^yearNumber) > in this case the equation becomes ($25*1.15%^1styear)= $28.749999999999996
For year 2 repeat the same process and do (startingPrice*interestRate^yearNumber) > this becomes ($25*1.15%^2ndyear)=$33.06249999999999
For year 3 again do (startingPrice*interestRate^yearNumber) > when plugging in numbers this becomes ($25*1.15%^3rdyear)=$38.021874999999994
For the 4th year the same process will be repeated (startingPrice*interestRate^yearNumber) > when plugging in this equates to($25*1.15%^4thyear)=$43.72515624999998 
The total balcance after 5 years can be calculated by using the same formula of (startingPrice*interestRate^yearNumber) > when plugging in this becomes ($25*1.15%^5thyear)= 50.283929687499985

Reflection: The first thing I did was set interestRate=float(input and then the question/command. I then divided this by 100 in order to convert the decimal into a percentage. I added 1 so when multiplying by the interestRate, the number would go up and not down. I did the same process for startingPrice by setting startingPrice equal to float(input( and then the question/command. For numberofYears I did the same thing but used int instead of float. The reason I did this is because there had to be a whole number of years. It wouldn't make sense to have 3.9 years in this problem as the total balance is being calculated after every whole year. For numberofYears after int I did (input( and then the question/command. I then added 1 to make sure there were 6 years caclulated beacuse the 0th year was included. If I didn't add one, there would have only been 5 years calculated and the 5th year would have really been the calculation for the 4th year. This is because of the inclusion of the 0th year. Next I wrote for yearNumber because I needed to change the number of years through each calculation. I then did in range(numberofYears): to make sure the yearNumber calculated was in the correct change of the numberofYears given. After this, I did print(startingPrice*interestRate^yearNumber).I did this as the startingPrice*interestRate^yearNumber would give the price for each individual year with compounding interest. To add each year could be caclulated seperately using the aforementioned formula. The most challenging thing was figuring out that I had to add one to the percentage to make the overall answer increase and not decrease. This was challenging because I normally just divide a number by 100 to get a percentage and not add anything. The most satisfying thing was checking the code and seeing there weren't any errors. This is because at first I had several errors that I had to work through and fix. 
 
