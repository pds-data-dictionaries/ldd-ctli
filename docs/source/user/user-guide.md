December 13, 2019
Lyle Huber

# Introduction

## Purpose of this User’s Guide
This guide describes the organization and contents of the Instrument Type (CTLI) Data Dictionary, one of several Data Dictionaries maintained by the Planetary Data System (PDS). This dictionary is used when creating labels for instrument context products. 

## Audience
This guide is intended primarily for use by PDS personnel (or their international equivalents). Context products should be both created and curated by the PDS.

## Applicable Documents
The Planetary Data System Standards Reference, [https://pds.nasa.gov/datastandards/documents/sr/current/](https://pds.nasa.gov/datastandards/documents/sr/current/), the complete reference for the PDS4 Information Model 
The PDS4 Data Dictionary, [https://pds.nasa.gov/datastandards/documents/dd/current/](https://pds.nasa.gov/datastandards/documents/dd/current/), the PDS4 core (or “common”) dictionary in an easily searchable HTML format 
The PDS4 Information Model Specification, [https://pds.nasa.gov/datastandards/documents/im/current/](https://pds.nasa.gov/datastandards/documents/im/current/), the same information as in the PDS4 core dictionary, in a formal specification for use by programmers and data engineers


# Overview of the {name} Local Data Dictionary

The Instrument Type Data Dictionary provides a way to classify instrument types. It also allows for similar types to be connected to each other to aid in search. This dictionary is only for use in instrument context products and so should only be used by PDS personnel when creating context products to associate with archive bundles.

# How to Include the {name} Local Data Dictionary in a PDS4 Label

```xml
     <Instrument>
         <name>Radio Science Subsystem</name>
         <Type_List_Area>
             <ctli:Type_List>
                 <ctli:type>Radio Science</ctli:type>
             </ctli:Type_List>
         </Type_List_Area>
 
         <naif_instrument_id>not applicable</naif_instrument_id>
         <serial_number>not applicable</serial_number>
         <description>
           The telecommunications system uses an X-band transponder on the spacecraft and
           transmitters and receivers at stations of the NASA Deep Space Network on Earth.
           Range and Doppler measurements made during communcations sessions can be used to
           determine the spacecraft trajectory; from the trajectory, Mercury's gravity field
           can be inferred.  Measurements of occultation times can be used to obtain the
           planet's radius at the occultation points, refining the planet's shape model.
         </description>
     </Instrument>

```


# Examples

TBD