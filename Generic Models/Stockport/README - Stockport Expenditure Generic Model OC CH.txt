Stockport Expenditure Generic Model
===========================

Status: ready/tested 
---------------
Last test: 6 February 2015

Overview
--------
A Refine project to model Stockport expenditure data and match suppliers to the Open Corporates and Companies House databases. User will need to edit select URIs and labels to ensure dates are appropriately assigned. Using the RDF skeleton on Open Refine, identify the following:

- 2nd Root Node [(Transaction Number URI)] -> [(row index) URI]
- 3rd Root Node [(row index) URI] -> [(row index) URI]
- 3rd Root Node [(row index) URI] -> [(row index)]
- 3rd Root Node [(row index) URI] -> [Clearing Date URI] -> [http://.../YYYY-MM]
                                  -> [Clearing Date URI] -> [http://.../YYYY-Q?]
                                  -> [Clearing Date URI] -> [http://.../YYYY-H?]
                                  -> [Clearing Date URI] -> [http://.../YYYY-YYYY] 

Click to open the greyed out boxes. In the bottom right section 'Use custom expression' section, click to open the 'preview/edit' box, and edit the dates using the appropriate format.

Upon applying the model, Refine will automatically start to reconcile with the OpenCorporates website. This may take a few minutes.

Please see video tutorials for a walkthrough on how to code Council spending data into linked data, and then upload to the GMDSP datastore.

Use case
--------

This could be applied to a dataset containing council expenditure information. For example

- Over £500 Spend Excel/CSV files
- http://www.stockport.gov.uk/services/councildemocracy/your_council/documentsandfacts/budgetsfinancialmonitoringreports/expenditureover500

Ontologies
----------
This work utilises the Data.Gov.Uk Payments Ontology to define types of payments and the bodies, departments and suppliers involved. Please refer to the following site for clarity on which label to use.

http://data.gov.uk/resources/payments/reference

Contents
--------
The package consists of:

- Example spreadsheet
- Example Open Refine project 
- Example output RDF file
- Example graph of RDF

Issues / 2do
------------

Stockport spend data does not contain specific dates for each transaction. All transactions have been assigned to the first day of the month. This may affect display of a data cube.