# Core project of the open-gdsn initiative

One of the major drawbacks of the GS1 Specifications regarding GDSN is the fragmentation of the specs. It is split up into XSD's , PDF documents and spreadsheets which requires a lot of reading, interpreting, combining before there is any useful overview that can be the basis of an implementation. This is all indicative of 'old-school' organisations that have their origin in the pre XML EDI era (ANSI X.12, EDIFACT) where you needed these kinds of documents to be actually descriptive enough for a real standard. 

###2016

It currently is 2016, XML and a huge set of related standards, including Schematron, has actually found its way into modern organisations that focus on the usage of business standards. So why not into GS1? I've heard some 'rumors' two years ago, but if an organisation like GS1 cannot produce a Schematron annotated XSD for the upcoming MJR3, I doubt it will ever come. Ans so if the mountain won't come to Muhammed, Muhammed must go to the mountain.

###Validations via Schematron

The first step in the open-gdsn initiative core project is to start implementing the [GDSN Validation Rules 3.1](http://www.gs1.org/gdsn/gdsn-validation-rules/3-1) *in* [the GS1 GDSN 3.1 schemas](http://www.gs1.org/gdsn/3-1#schemas) via Schematron annotations. It will be a two phase approace where The focus will initially be on the [Catalog Item Synchronization ](http://www.gs1.org/docs/gdsn/3.1/BMS_GDSN_Catalogue_Item_Sync_r3p1p0_d1_p0_p4_18dec2013_Implementers_Packet.zip) starting with the TradeItem.xsd and when that is finished, and only then the additional [Trade Item Modules](http://www.gs1.org/gdsn/gdsn-package-trade-item-modules-bms/3-1) will be augmented.
