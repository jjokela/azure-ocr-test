# azure-ocr-test
Testing Azure OCR functionality

This python sample reads the following example trade confirmation file, and uses the Azure OCR to get the text contents out of it. [Trade confirmation file](https://www.vmdconseil.ca/Documents/transaction-anonyme.pdf)

[Azure Quickstart link](https://docs.microsoft.com/en-us/azure/cognitive-services/computer-vision/quickstarts-sdk/client-library?tabs=visual-studio&pivots=programming-language-python)

This is a modified python quickstart sample.
What you need:
- Azure account
- create Computer Vision resource in your account

Clone the repo, install following packages:
- `pip install --upgrade azure-cognitiveservices-vision-computervision`
- `pip install pillow`

In the code, replace the key and endpoint of your own Computer Vision resource:
- `subscription_key = 'XYZ'`
- `endpoint = 'ABC'`

Then run the sample.

You get back the following result:
```
<snip>
We confirm the following activity on your account number:
Transaction Details
Transaction
Account Number:
Quantity Bought
Quantity Sold |Description
Unit Price ($)
Date
Number:
10 BANK OF NOVA SCOTIA
68.96
RR:
RRIF PAYMENTS
SM1501861
Symbol:
BNS
UNSOLICITED
CUSIP:
064149107
Security Code:
055897
Transaction Amount:
$2,758.40

...
```
