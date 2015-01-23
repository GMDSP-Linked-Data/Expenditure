Trafford Expenditure Generic Model
===========================

Status: ready/tested 
---------------
Last test: 22 January 2015

Overview
--------
A Refine project to model Manchester expenditure data. User will need to edit select URIs and labels to ensure dates are appropriately assigned. Using the RDF skeleton on Open Refine, identify the following:
- 2nd Root Node [(Transaction Number URI)] -> [(row index) URI]
- 3rd Root Node [(row index) URI] -> [(row index) URI]
- 3rd Root Node [(row index) URI] -> [(row index)] 
- 3rd Root Node [(row index) URI] -> [Date URI] -> [http://.../YYYY-MM]
                                  -> [Date URI] -> [http://.../YYYY-Q?]
                                  -> [Date URI] -> [http://.../YYYY-H?]
                                  -> [Date URI] -> [http://.../YYYY-YYYY]

Click to open the greyed out boxes. In the bottom right section 'Use custom expression' section, click to open the 'preview/edit' box, and edit the dates using the appropriate format.

Use case
--------

This could be applied to a dataset containing council expenditure information. For example

- Over £0 Spend Excel/CSV files
- http://www.trafford.gov.uk/about-your-council/data-protection/open-data/open-data.aspx

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

Ready for use.