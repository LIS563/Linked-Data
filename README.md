# Linked-Data

Author: Mary Currier

Date of ReadMe File Creation: April 10, 2026

Sources for Related Data: MARC Records Datasets, Revised Graph.png, Linked_Data_Mapping_Template Revised, and MARC_Records_Data.ttl.
                          Upon opening MARC Records Datasets in the GitHub account, more library suggested items could be added to the 
                          spreadsheet.
                          
##Dataset Description

The dataset for this linked data project is based on both non-fiction and fiction books or authors of personal interest to me from my local public library.  Each separate item (book) has a space provided for each of these certain MARC fields that identify a book easily, if included in the MARC record, such as: ISBN, Library of Congress call number, Dewey Decimal Classification call number, Author, Title, Alternative title, Edition information, and Physical description data. The spreadsheet is similar to one that might be made by librarians for an acquisitions librarian in order to suggest possible books to purchase for a library's collections.

##Ontologies or Controlled Vocabulary Used

The data is all related to books for libraries, so BIBFRAME or Dublin Core were the best choices to consider as a possible vocabulary for the project.  Since Dublin Core is likely simpler to understand than BIBFRAME, and I've already worked with this vocabulary in a previous class, that was a choice made with no thought required.

##Linking Strategy

All of the fields in the dataset were linked to Dublin Core vocabulary, and the only field that had a URI that I reconciled was the Author field (dcterms:creator), which could often easily be matched to the exactly correct author name from VIAF.  The other seven fields in the dataset were literals, with a datatype or a language tag.

##Sample Triples


dcterms:Creator       ---has Written--->       dcterms:Title

Charles Todd -                                  A Test of Wills

viaf:  79485267 ;



dcterms:Creator       ---has Written--->       dcterms:Title

Charlaine Harris -                               Real Murders

viaf:  50289397 ;



dcterms:Creator       ---has Written--->       dcterms:Title

Bryan Stevenson -                                 Just Mercy

viaf:  54144648307661510122 ;
       


