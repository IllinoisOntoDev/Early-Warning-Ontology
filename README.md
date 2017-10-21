# Domain Description 

## Scope of the proposed area
With the advent of new geospatial technologies, tracking real-time criminal activities has become a prevalent practice. Some existing platforms such as [Criminal Reports](https://www.crimereports.com/) provides such statistics and data within a period of time; while governmental warning systems (e.g. Illini alert) receives criminal activity reports and sends warning messages via text messages or social media. However, these warning systems usually still deferred a little when sending out the warnings; and the messages are sent to the mass public when only selected areas were affected.

Previous research has dwelled on building early warning systems for **tsunamis** (Ramar & Mirnalinee, 2012). Others focused on _crisis management_ or _disaster prevention_, but still mainly in the domains of natural disasters, with an emphasis on providing sensor ontologies that can identify signals, wave lengths, timestamp, and other signal processing relevant features (Liu et al., 2013; Klien, Lutz, & Kuhn, 2006; Poslad et al., 2015). 

Building early warning ontologies for human activities such as crime events has not yet been seen. In this research, I would like to develop a **geospatial ontology for crime activities early warning**. With the help of ontologies, we may be able to:

(1)	Use the reasoning and inference fuction in ontologies and infer the ‘affected’ zones of the criminal activities 

(2)	Use the time-related classes and properties to track the activities without time-delay

Crime activities are in a way _crisis management_, which echoes what Liu et al. (2013) said that the infrastructure may be complex because we have to take into account the timeframe of events. That is, we need to have corresponding information for before, during, or even after the crime crisis. 

Ontology can be useful in that sense because it provides rich semantic descriptions, therefore reduces the semantic heterogeneity problems occurs in systems that do not have well-constructed data structure (Klien, Lutz, & Kuhn, 2006; Liu et al, 2013; Ramar & Mirnalinee, 2012). Poslad et al. (2015) further elaborated that the semantics in ontologies can help us define more precisely the terms and relationships between complex concepts in the disaster warning workflow, while on the other hand leading to a stronger rule-based inferencing and can enhance “service interoperability, orchestration and extension”. 

## Relationships to the case study

With the following information provided in the Jail Dataset case study, we may be able to link it with the real-time criminal activity ontology: 

**(1) Location information**   

Information in columns such as _zip code, city, state_ is highly relevant to creating geospatial ontologies. If we can utilize these information and link it with actual coordinates (longitude and latitude), we may be able to deduce more precisely the areas that were affected by some criminal incidents. 

**(2)Time information**

Timestamps as to when the prisoners were brought into jail is also very crucial to building our ontology. We may be able to make good use of information such as the _booking date, booking time, days in Jail, hours, minutes, second,_ and _release dates_ columns. Though they may not contribute to the ‘real-time’ tracking, these information can still be very valuable when we want to further track individuals who have committed serious crimes- to know that they have/ have not yet been released.


**(3)Type of crimes**

Type of crimes (e.g. the _CrimeCode_ column) is also pertinent information to our ontology. Our aim is to find not when and where, but also what kind of things happened in that space; so distinct Crime Code can serve as the classes of our ontology. 


## Existing published vocabularies that are candidates for extension or adaptation

**(1)	GeoNames**

In Liu et al. (2013)’s review of the state of the art crisis management ontologies, they concluded that few crisis ontologies are ‘formally represented’, even among the ones that are in the form of ontologies (such as SOKNOS, IsyCri, WB-OS), they are not open to public. However, for the geospatial domain, the authors recommend the reuse of [GeoNames](http://www.geonames.org/) as a best practice, because GeoNames offers extensive resource for toponyms. 

**(2) GeoSPARQL**

The Open Geospatial Consortium (OGC) provides a series of standards and best practice for publishing geospatial data online, one of which is the use of [GeoSPARQL](http://www.opengeospatial.org/standards/geosparql). GeoSPARQL supports querying geospatial data in RDF, and may be a potential candidate for our crime activities early-warning ontology. 

**(3)Others**

In the W3C Geopsptatial Ontologies report (2006), other existing vocabularies or ontologies we may consider to adapt are: 
-	WGS84 standard for coordinate reference system
-	RCC-8 (Region Connection Calculus) for topological relationships between terms
 
Other ones such as the [Getty Thesaurus of Geographic Names](http://www.getty.edu/research/tools/vocabularies/tgn/index.html
) is also highly relevant. 


## Ideas for classes and properties
