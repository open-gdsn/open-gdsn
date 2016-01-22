# open-gdsn
A soon to be launched attempt to create a open and free (for non commercial companies) implementation in java. 

Initially it will consist of 

 - DataSource client (non-ui) for communicating with a certified SourceDataPool that supports the GDSN flow of messages
 - DataSource UI extending the DataSource client
 - DataRecipient client (non-ui) for communicating with a certified RecipientDataPool that supports the GDSN flow of messages
 - DataRecipient UI extending the DataRecipient client
 
Both clients will be based on a the same code and will initially support:

 - All GDSN Global validation rules (including conditionally required fields or allowed values)
 - A view for all GDSN fields
 - Sending (DataSource) or receiving (DataRecipient) CIN messages
 - Sending (DataSource) CIP messages
 - Sending (DataRecipient) or receiving (DataSource) CIC messages
 - Sending (DataRecipient) CIS messages
 - Customize views based on target market
 - Customize validations (Global, targetMarket based, or fully custom)
 - Adding custom fields for internal use that won't get send to the datapool
 - Allowing to import data from a backoffice and add/populate additional fields before sending the data to the DataPool (merging) and keeping the added data in tact after an additional import
 - Running in a 'mixed mode' configuration so wholesale companies can receive data from the datapool and use that data to forward it to their retailers
 
Ofcourse all basic things you expect from a solution like this are supported

 - searching
 - filtering
 - exporting
 - mass-update fields
 - status overview
 - error reporting 
 
**Future ideas**

We think all the above is a great basis for a usable solution, but we certainly already have ideas for the future
 
  - support for templating
  - saving/using custom filters
  - fully dynamic views based on e.g. GPC code
  - ability to send data to different datapools
  - support import mappings so custom formats can be uploaded

**Goal**

The idea is that after an initial release of the DataSource and DataRecipient parts, a real full blown GSDSN compliant DataPool will be implemented too. One of the biggest challenges for this will be the costly [Drummond certification](https://www.drummondgroup.com/b2b-certified-products/b2b-standards/gdsn) that is required by GS1

