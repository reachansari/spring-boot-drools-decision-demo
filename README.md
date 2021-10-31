# spring-boot-drools-demo
Spring boot drools for the input validations.

## Rest Controller
The class `CurrencyController.java` contains the endpoint.

**AVAILABLE ENDPOINTS**

| method            | resource          | response                                                                                   |
|:------------------|:------------------|:----------------------------------------------------------------------------------------------|
| `GET`			| `/currencyCode/SGD`		| Singapore Dollar													|
| `GET`			| `/currencyCode/SG1`	| { "code": 404, "errorMessages": "Invalid Currency Code. Must be a valid 2 letter alphabet." 	}				|
| `GET`			| `/currencyCode/IRR`		| Currency code not found														|


## Exception Handling
An Spring Boot advice `RestExceptionHandler.java` has been created for handling exceptions and convert them into desired responses.

| exception										| response     				   			|
|:----------------------------------------------|:--------------------------------------|
| `AddressNotFoundException`						| `404 NOT FOUND`					|



## Libraries used
- Spring Boot
- Spring Configuration
- Spring REST Controller
- Development Tools

	
## Compilation Command
- `mvn clean install` - Plain maven clean and install
