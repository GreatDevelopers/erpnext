# Documentation of Stock Module.

The Stock or Inventory module in ERPNext helps you to:

* Maintain details of your products and warehouses.
* Track receipt, transfer and delivery of the products.
* Optimize stock levels by providing real-time information via reports.
* Provide valuation of each product.

**First of all, Create Item Groups, Items, Warehouses, Suppliers etc.**

## Item Group:
An Item Group is a way to classify items based on types. Following are steps to create item group:
1. Go to the Item Group list, click on New.
2. Select a group node under which you wish to create the Item Group, the default root is 'All Item Groups'.
3. Select 'Add Child' or click on the New button.
4. To make this child a category/group node, tick on Group Node.
5. Click on Create New.

## Item:
An Item is a product or a service offered by your company. Following are the steps to create items:
1. Go to Stock -> Item.
2. Click on Add Item.
3. Keep the “Maintain Stock” field checked.
4. Save
(After saving, Stock Entry, Stock Ledger, Accounting Ledger will be created automatically.)

## Warehouse:
A warehouse is a commercial building for storage of goods. Warehouses are used by manufacturers, importers, exporters, wholesalers, transport businesses, customs, etc. Following are steps to create warehouse:-
1. Go to the Warehouse list, click on New.
2. Enter a name for the Warehouse.
3. Set/check the Parent Warehouse. If you tick on 'Is Group', you can create sub-Warehouses under this group Warehouse.
4. Save.

You can set a default account for all transactions with this warehouse. After saving a Warehouse, you'll see the following options:

Stock Balance: This will open the Stock Balance report to display the quantity, valuation, balance, etc.
General Ledger: This will open the General Ledger to display the accounting transactions.
Non-Group to Group: If the Warehouse is a Non-Group Warehouse, i.e. cannot contain other Warehouses under it, this button will make this a Group Warehouse.

## Supplier:
Suppliers are companies or individuals who provide you with products or services.
1. Go to the Supplier list and click on New.
2. Enter a name for the supplier.
3. Select the supplier group.
4. Save.
5. Create New Address and New Contact.
6. In New Contact, if the supplier is already a user of erp then select the user id otherwise enter email id in contact details. 
7. Then click on “Invite as User” then email will be sent to this email to set up the password.
8. Supplier will become a user now.

# Steps for creating stock:-

If the item is non serialized/non batched or the item is serialized and Serial Number Series is defined for a particular item, then add an entry in “Stock Reconciliation”. 

**Steps for creating Stock Reconciliation:**
1. First, Go to Stock -> Stock Reconciliation and click on “Add Stock Reconciliation”.
2. Select the “Purpose” as “Opening Stock”.
3. Enter all required data like Items, Warehouses, Quantity of Items etc.
4. Save.

If the item is serialized/batched then add an entry in “Stock Entry”

**Steps for creating Stock Entry:-**
1. First, Go to Stock -> Stock Entry and click on “Add Stock Entry”.
2. Select “Material Receipt” in “Stock Entry Type” field.
3. Fill the required data.
4. Define Serial Number or Batch Number of items.
5. Save.
(After adding an entry in Stock Reconciliation or Stock Entry, the item with specified quantity will be added in stock. You can check it in the Stock Ledger Report.)

# Steps to buy an item:-

1. First, Go to Stock -> Material Request and click on “Add Material Request”.
2. Select “Purchase” in the Purpose field and enter the required data.
(Note: You can create it manually or through re-order item in items list i.e. If item quantity goes below the re-order level of item then material request will be created automatically.
3. Save the document then Submit it.
4. Click on Create -> Request For Quotation.
5. All details will be fetched in the Request For Quotation document. Add the suppliers you want and fill the required fields.
6. Then click on Save and Submit.
(An email will be sent to the supplier with the "Supplier Quotation" link. From this link, Suppliers can submit their quotations. Then these quotations will be visible in the "Supplier Quotation" list.)
7. Open Supplier Quotation and submit it.
8. Now, Click on Create -> Purchase Order. 
(A Purchase Order is a binding contract with your Supplier that you promise to buy a set of items under given conditions).
9. Fill the required data and save it.
10. Now, Click on Create -> Purchase Receipt.
11. Enter the required data and submit it.
(After creation of Purchase Receipt, Items will be added in the warehouses. You can check the item's entry in the Stockh Ledger Report.)
12. Click on Create -> Purchase Invoice. 
(A Purchase Invoice is a bill you receive from your Suppliers against which you need to make the payment)
(You can check Invoice Amount, Outstanding Amount, Paid amount etc. in "Account Payable")
13. Now, Click on Create -> Payment.
14. Choose the Mode of Payment and fill the required fields.
15. Click on Save -> Submit.
(After paying, Invoice status will be changed to "Paid" and also now this invoicewill not be available in the Account Payable Report.)



# Documentation of Asset

**Asset:** In ERPNext, you can maintain fixed asset records for Company assets like computers, furniture, cars, etc. and manage their depreciations, sale. It is any valuable item owned by a company.
Asset category: Asset Category based on the type of assets. For example, all desktops and laptops can be part of an Asset Category named 'Electronic Equipments'.

To access the Asset list, go to:
Home > Assets 

## How to create an Asset
An Item representing the asset should be created. The 'Maintain Stock' should be unchecked and 'Is Fixed Asset' must be checked.

**1. Auto creation of assets**

You can configure ERPNext to automatically create assets on submission of Purchase Receipt by enabling 'Auto Create Assets on Purchase' in Item.
If you have enabled auto asset creation for the item representing an asset, you will have to provide the asset location while submitting the Purchase Receipt.
A message confirming the creation of assets is displayed on submission of Purchase Receipt.

**2. Manual creation of assets**

If you would like to create assets manually, create an Item with 'Is Fixed Asset' enabled and leave 'Auto Create Assets on Purchase' unchecked . On submission of a Purchase Receipt/Purchase Invoice with that Item a message is shown indicating that you need to create assets manually.

Follow below steps to create assets manually.
1. Go to the Assets list, click on New.
2. Enter a name for the asset.
3. Select the Item Code. Item Name and Asset Category will be fetched automatically.
4. Select the Asset Owner, i.e. Company, Supplier, or Customer.
5. Select the Company/Supplier/Customer.
6. Select the Purchase Receipt/Purchase Invoice. Purchase Date and Gross Purchase Amount will be fetched automatically.
7. Select a Location. Eg: Mumbai Office. This will be fetched automatically if specified in Purchase Receipt items table
8. Set Available-for-use Date. The depreciation will be calculated starting from this date.
9. Save and Submit.
Please note you need create one asset record for each asset you have bought. If you have bought five computers and have created just one Purchase Receipt with quantity set to five then you will have to create five asset records manually.
 
**3. Importing existing assets**

When you move from a legacy system to ERPNext, you will have to add details of all the assets your company has purchased previously along with depreciation details of each asset.
For an existing asset, you can create the asset record directly by checking "Is Existing Asset" checkbox and provide below details.
* Gross Purchase Amount
* Purchase Date
* Available-for-use Date
* Opening Accumulated Depreciation: The accumulated depreciation amount which has already been booked for an existing asset.
* Number of Depreciations Booked: Number of depreciation entries already booked.
