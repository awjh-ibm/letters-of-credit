# Scenario
In this sample you will take on the role of four participants to see how blockchain can be used to track letters of credit. These participants are:

**Alice Hamilton** - Owner of QuickFix IT, a company specialising in the sale of computers.

**Bob Appleton** - Owner of Conga Computers, a manufacturer of computers.

**Matías** - Employee of Penguin Bank, the bank which Alice has an account with.

**Ella** - Employee of the Bank of Hursley, the bank which Bob has an account with.

The above participants have varying roles in the scenario with Alice playing the *applicant*, Bob the *beneficiary*, Matías the *issuing bank* and Ella the *exporter bank*.

In the scenario that this sample covers Alice and Bob have agreed that Alice will purchase computers from Bob's next shipment and have agreed a price for these. Alice unfortunately does not have enough money in her account to cover the entire cost of the purchase and therefore she is requesting a letter of credit to cover this cost from her Bank, Penguin Bank. This sample will cover how this letter of credit is tracked using blockchain.

# Tutorial

## Setting up the demo
Open each participant's application in a seperate tab. [Alice's banking app](%LETTER_OF_CREDIT_APP%/alice), [Matías' employee bank view](%LETTER_OF_CREDIT_APP%/matias), [Ella's employee bank view](%LETTER_OF_CREDIT_APP%/ella) and [Bob's banking app](%LETTER_OF_CREDIT_APP%/bob).

## Applying for a letter of credit

On Alice's screen apply for a new letter of credit. 

Enter the product details the letter of credit will cover by clicking 'Edit', entering computers for the type, 100 for the quantity and 1200 for price per unit. Save your changes.

Review the terms and conditions then confirm the request for a letter of credit by clicking 'Start approval process' and pressing 'Yes' to the modal warning.

Note: For the purpose of this sample the details of Bob are prefilled in for the letter of credit. 

## Issuing bank approval

Navigate to Matías' screen and you will see that there is a new request for a letter of credit from Alice Hamilton. Click on the request to view it in full. 

Review the product details and terms and conditions and then accept the application by clicking 'I accept the application' and pressing 'Yes' to the modal warning. 

## Exporting bank approval

Once the issuing bank has approved the letter of credit it is now visible to Ella. 

Navigate to Ella's screen and you will see that there is a new request for a letter of credit from Alice Hamilton awaiting approval. Click on the request to view it in full. 

Review the product details and terms and conditions are acceptable and then accept the application by clicking 'I accept the application' and pressing 'Yes' to the modal warning.

## Exporter approval

Now that the letter of credit has been approved by both the issuing bank and the exporter it is now visible to Bob. Navigate to Bob's screen and click 'View Letter of Credit'.

Review the product details and terms and conditions are acceptable and then accept the application by clicking 'I accept the application' and pressing 'Yes' to the modal warning.

## Declaring the goods as shipped

When Bob has shipped the goods he can use his banking application to update the letter of credit with information regarding this.

Within Bob's screen click 'Ship Order' to mark that the goods have been shipped.

This writes to the letter of credit a hash of his shipping documents for use as proof. 

## Declaring the good as received

Once Bob has shipped the goods Alice can then mark when she receives the goods that she accepts the order. By clicking accept order Alice agrees that what she has received matches the terms set out for the goods in the letter of credit. 

In Alice's screen click 'Accept Order'.

## Issuing payment
Once Alice has marked the goods as received Matías is alerted to this through his employee banking application. The issuing bank will then performs their own check on the goods and pay the letter of credit if they agree that they match the terms laid out in the letter of credit.

On Matías' screen click the letter of credit and press 'Ready for payment' and press 'Yes' to the modal warning.

## Closing the Letter of Credit
Now that the issuing bank has confirmed that they are happy with the goods and have made the payment the exporter bank can close the letter of credit and deposit the funds to the beneficiary. 

In Ella's screen click the letter of credit and press 'Close this letter of credit'.

## Confirming completion
Now that the letter of credit is closed Bob will have had the value of it deposited in his account. 

On Bob's screen review his bank balance and note that the payment has been made.

# Next steps
This sample was built using [IBM Blockchain Platform: Develop](https://console.bluemix.net/docs/services/blockchain/develop.html#develop-the-network). Check out the model and business logic behind this sample [here](%PLAYGROUND_URL%), or browse the generated REST APIs [here](%REST_SERVER_URL%).