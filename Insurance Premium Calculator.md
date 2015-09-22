## Insurance Premium Calculator
Reads users profile info from a text file, does calculations, displays results.


##Methods (in addition to main):*```java
readTextFile() : A method that reads the PolicyInformation.txt file.
``` 
```java
public static double calculateFinalPolicyPrice(int age, bool isSmoker, double bmi){
// logic to calculate the final price

double baseRate = 400;
IF age is greater than 50 THEN
	add $100.00 to baseRate
ENDIF
IF isSmoker is true THEN
	add $150.00 to baseRate
ENDIF
IF calculatedBMI is over 40% THEN
	add $100.00 to the baseRate
ENDIF

int totalPrice = baseRate;

return totalPrice
}

//A method that accepts argument(s) and will calculate and return the final price of a single customer’s insurance premium. Calculate the premium using the table on page 2.```

```java
A method that calculates and returns a customer's BMI.
public static double getCustomerBMI(double height, double weight){
//todo: logic to calc BMI
double bmi = (weight * 703) / (height^2);

return bmi;
}```

```java
public static double getTotalInsurancePremiums()

A method that will calculate and return the total price of all insurance premiums. ```

```java
public static string displayAllPolicies(){


return allPolicies;
}

A method that displays the policy information as shown in the sample output on page 3 of this document.  ```

### Sample Input Data
Let's identify what type we should use to represent each item inside of the text file that holds the data of each customer



| Field Name  | Data Type  | Variable Name |
|:------------- |:---------------:| -------------:|
| Policy Number      | Integer |   policyNumber |
| Provider Name    | String(text)     |   providerName |
| First Name | String(text) |            firstName |
| Last Name | String(text)       |            lastName |
| Age | Integer   |        age |
| Smoking Status | Boolean (true or false)    |    isSmoker |
| Height (in.) | Double    |            height |
| Weight (lbs) | Double   |      weight |
| BMI (Body Mass Index) | Double    |            bmi |
| Insurance Premium Cost | Double   |       premiumCost|


####Example Data
```
3450 - Policy Number
State Farm - Provider Name
Alice - First Name
Jones - Last Name
20 - Age of the Customer
smoker - isSmoker = true
65 - BMI of Customer
110 - weight of the customer
```

## Premium Table These values are used to calculate the Premium of a policy for a user.- Base rate -- > $400- Over 50	Add $100 - Smoker	Add $150 - BMI over 40	Add $100 - A bmi is calculated as weight times 703 divided by height2. ### What can we identify from the premium table?
Let's find some variables from this data.

```java
double baseRate = 400;
IF age is greater than 50 THEN
	add $100.00 to baseRate
ENDIF
IF isSmoker is true THEN
	add $150.00 to baseRate
ENDIF
IF calculatedBMI is over 40% THEN
	add $100.00 to the baseRate
ENDIF

```