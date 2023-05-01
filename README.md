# isFraud-Competition

The goal of the project is to select and create the best prediction algorithm to predict whether a certain transaction is fraudulent or not. This is the first project of Machine Learning Models course.

#### Structure of the notebook:
* `Libraries`: Includes a briefly description of where they were used in the process
* `Data Export`: Includes the data export, separation in train-test and exploration
* `Cleaning Pipelines`: Building of the three pipelines that I used
* `Model`: Building of the pipeline where I'm placing my model
* `Saving Model Pipeline`: Saving the pipeline where I built my model

#### Description of the repo:
* `FraudModel.pkl`: The file which contains the model created
* `Test.csv`: The dataset without the variable *isFraud*
* `Train.csv`: The dataset with the variable *isFraud*, which is the variable to predict. This dataset was used to create the model
* `script.ipynb`: Jupyter Notebook with all the creation process
* `solutions.csv`: A CSV file with the answers. This competition was submitted in Kaggle and it requiered a specific format to upload the answers

#### Variables (I didn't used all of them):
* `accountNumber`: client's account number
* `customerId`: client's individual id
* `creditLimit`: credit limit of the client
* `availableMoney`: available credit
* `transactionDateTime`: date and time when the transaction occured
* `transactionAmount`: amount of the transaction
* `merchantName`: name of the business where the transacction occured
* `acqCountry`: country code where the transaction occured
* `merchantCountryCode`: contry code where de business is located
* `posEntryMode`: POS lecture mode, it could be: 
  * 02 - PAN auto-entry via magnetic stripe, track data is not required, 2 - no PIN.
  * 05 - PAN auto-entry via chip, 2 - no PIN.
  * 09 - E-Commerce, 0 - unknown PIN capability.
  * 80 - Fallback to magnetic stripe, 0 - unknown PIN capability.
  * 90 - PAN auto-entry via magnetic stripe, track data should be transmitted within the authorization request.
* `posConditionCode`: aditional conditions when the transaction occured, it could be:
  * 01 - Cardholder not present
  * 08 - Mail/telephone order (includes Visa phone and reoccurring transactions)
  * 99 - Other
* `merchantCategoryCode`: the type of business where the transaction occured
* `currentExpDate`: expiration date of the card
* `accountOpenDate`: date in which the bank account was opened
* `dateOfLastAddressChange`: date in which the physical address was changed
* `cardCVV`: real CVV code
* `enteredCVV`: CVV code received during the transaction
* `cardLast4Digits`: last 4 digits of the card
* `transactionType`: type of transaction
* `currentBalance`: amount of money available in the card when the transaction occured
* `cardPresent`: if the card was there during the transaction
* `expirationDateKeyInMatch`: if expiration date card is older than transaction date
* `isFraud`: transaction was fraud or not (variable to classify)
