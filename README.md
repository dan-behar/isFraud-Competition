# isFraud-Competition

The goal of the project is to select and create the best prediction algorithm to predict whether a certain transaction is fraudulent or not. This is the first projecto of Machine Learning Models course.

#### Structure of the notebook:
* `Libraries`: Includes a briefly description of where they were used in the process
* `Data Export`: Includes the data export, separation in train-test and exploration
* `Cleaning Pipelines`: Building of the three pipelines that I used
* `Model`: Building of the pipeline where I'm placing my model

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
** 02 - PAN auto-entry via magnetic stripe, track data is not required, 2 - no PIN.
05 - PAN auto-entry via chip, 2 - no PIN.
09 - E-Commerce, 0 - unknown PIN capability.
80 - Fallback to magnetic stripe, 0 - unknown PIN capability.
90 - PAN auto-entry via magnetic stripe, track data should be transmitted within the authorization request.
posConditionCode:
01 - Cardholder not present
08 - Mail/telephone order (includes Visa phone and reoccurring transactions)
99 - Other
merchantCategoryCode: categoría del comercio donde se hace el consumo
currentExpDate: fecha de expiración de la tarjeta
accountOpenDate: fecha en la que se abrió la cuenta en el banco
dateOfLastAddressChange: fecha del último cambio de dirección
cardCVV: código real detrás de la tarjeta
enteredCVV: código ingresado detrás de la tarjeta
cardLast4Digits: últimos 4 dígitos de la tarjeta
transactionType: tipo de transacción
currentBalance: refleja todos los cargos y la actividad de pago en la cuenta de tarjeta de crédito hasta la fecha en que se generó el estado de cuenta
cardPresent: la tarjeta de crédito estuvo presente o no en la transacción
expirationDateKeyInMatch: la fecha de expiración de la tarjeta es anterior a la transacción
isFraud: la transacción es fraude o no (variable a clasificar)
