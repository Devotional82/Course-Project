# Course-Project
Strong password variation
(String with special characters, letters and digits)
import random
import string

def randomStringwithDigitsAndSymbols(stringLength=10):
    password_characters = string.ascii_letters + string.digits + string.punctuation
    return ''.join(random.choice(password_characters) for i in range(stringLength))

print("Generating Random String password with letters, digits and special characters ")
print ("First Random String ", randomStringwithDigitsAndSymbols() )
print ("Second Random String", randomStringwithDigitsAndSymbols(10) )
print ("Third Random String", randomStringwithDigitsAndSymbols(10) )
Generating Random String password with letters, digits and special characters 
First Random String  &<lXovwux"
Second Random String oSM/L3je4&
Third Random String [2j;WF.3hr

(Generating a secured random string)
import string
import secrets
def random_secure_string(stringLength):
    secureStr = ''.join((secrets.choice(string.ascii_letters) for i in range(stringLength)))
    return secureStr
print("First secure random String is ", random_secure_string(6))
print("Second secure random String is ", random_secure_string(6))
First secure random String is  erLWPs
Second secure random String is  CSYVhN

(Generate a secured token string)
import secrets
print("Secure hexadecimal string token", secrets.token_hex(32))
Secure hexadecimal string token 3213bef2cc356c0cf6a9f27b4b36d943fecfe93bec6ea42fc1289bc8115d5fc2

(UUID module to generate Universally Unique secure random String Id)
import uuid
stringId  = uuid.uuid4()
print("Secure unique string Id", stringId)
Secure unique string Id 0d6d239d-32bb-4562-a4f6-2c18ead8f637

The End
