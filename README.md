# RxObject.js v1.1
A javascript object for spectacle prescription parameters
The string property is for input and display
The vector property is for storage and manipulation
String and vector are always in sync

# Constructor
If input is a string, the object will validate the string against the validation parameter or a default
If input is a number, no validation is done.
use obj= new RxObject(string input, string type, [string validation])
Allowed types: sph, cyl, axisC
Allowed validations: 0.25, -0.25, 0.12, -0.12, 180

# Get Methods
getString() - a string
getVector() - a number
getValidation() - boolean true|false
getValidationMsg() - a string

# Set Methods
You cannot set a type - a new object must be constructed to change the type

setString()
Updates string and vector properties after validation
use obj.setString(string input,[string validation])
returns
setString().result - boolean true|false
setString().msg - string
if setString() is successful,all obj properties are updated
