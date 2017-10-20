# Domain Description 

## Scope of the proposed area
With the advent of new geospatial technologies, tracking real-time criminal activities has become a prevalent practice. Some existing platforms such as [Criminal Reports](https://www.crimereports.com/) provides such statistics and data within a period of time; while governmental warning systems (e.g. Illini alert) receives criminal activity reports and sends warning messages via text messages or social media. However, these warning systems usually still deferred a little when sending out the warnings; and the messages are sent to the mass public when only selected areas were affected.

In this research, I would like to develop a geospatial ontology for tracking real-time criminal activities. With the help of ontologies, we may be able to:

(1)	Use the reasoning methods in ontologies and infer the ‘affected’ zones of the criminal activities 

(2)	Use the time-related classes and properties to track the activities without time-delay

## Relationships to the case study

With the following information provided in the Jail Dataset case study, we may be able to link it with the real-time criminal activity ontology: 

**(1) Location information   

Information in columns such as _zip code, city, state_ is highly relevant to creating geospatial ontologies. If we can utilize these information and link it with actual coordinates (longitude and latitude), we may be able to deduce more precisely the areas that were affected by some criminal incidents. 

**(2)Time information

Timestamps as to when the prisoners were brought into jail is also very crucial to building our ontology. We may be able to make good use of information such as the _booking date, booking time, days in Jail, hours, minutes, second,_ and _release dates_ columns. Though they may not contribute to the ‘real-time’ tracking, these information can still be very valuable when we want to further track individuals who have committed serious crimes- to know that they have/ have not yet been released.


**(3)Type of crimes

Type of crimes (e.g. the _CrimeCode_ column) is also pertinent information to our ontology. Our aim is to find not when and where, but also what kind of things happened in that space; so distinct Crime Code can serve as the classes of our ontology. 



## Existing published vocabularies that are candidates for extension or adaptation

https://www.w3.org/TR/sdw-bp/#linking

https://www.w3.org/2005/Incubator/geo/XGR-geo-ont-20071023/


## Ideas for classes and properties
