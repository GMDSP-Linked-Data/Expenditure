Tameside Expenditure Generic Model
===========================

Status: ready/tested 
---------------
Last test: 6 February 2015

Overview
--------
A Refine project to model Manchester expenditure data and match suppliers to the Open Corporates and Companies House databases. User will need to edit select URIs and labels to ensure dates are appropriately assigned. Using the RDF skeleton on Open Refine, identify the following:

- 2nd Root Node [(Inv Transaction URI)] -> [(row index) URI]
- 3rd Root Node [(row index) URI] -> [(row index) URI]
- 3rd Root Node [(row index) URI] -> [(row index)] 
- 3rd Root Node [(row index) URI] -> [Paid Date URI] -> [http://.../YYYY-MM]
                                  -> [Paid Date URI] -> [http://.../YYYY-Q?]
                                  -> [Paid Date URI] -> [http://.../YYYY-H?]
                                  -> [Paid Date URI] -> [http://.../YYYY-YYYY]

Click to open the greyed out boxes. In the bottom right section 'Use custom expression' section, click to open the 'preview/edit' box, and edit the dates using the appropriate format.

Please see video tutorials for a walkthrough on how to code Council spending data into linked data, and then upload to the GMDSP datastore.

Use case
--------

This could be applied to a dataset containing council expenditure information. For example

- Over £500 Spend Excel/CSV files
- http://www.tameside.gov.uk/transparency/archive

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

Tameside October 2014 caused problems with upload. All other data has been successfully modelled.