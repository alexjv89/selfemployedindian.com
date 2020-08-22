# How to create recurring invoice via zoho invoice?

If you are billing the same about to the client every month, then the recurring invoice feature of zoho invoice is a very useful feature. 

Creating recurring invoice:

- Create a customer 
- Create a recurring invoice from the UI.  
	- Choose repeat duration - monthly/ weekly/ quarterly etc
	- Choose start date
	- Choose end date or never expires
	- Enter line item


## How to add variability to your line items

Lets say you want to specific the month in the line items. Invoice date is not always a reliable way to figure out which period are you billing for. What I do is, I specify the period in the line items. Zoho invoice supports variables. 

`For %(m)(Year)%`

## Most common use case - billing on 28th of the month for the current month

Set the start on date to 28th.

Create an item called `consulting`

In the description, type this - `For %(m)(Year)%` . It will show up as - `For August 2020`