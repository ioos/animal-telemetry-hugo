+++
weight = "20"
type = "post"
draft = false
sidebar = true
date = 2014-03-04T07:56:39Z
title = "A Metadata Convention for Passive Acoustic Recordings"

+++

_The objective of this document is to present metadata that supports the mission of the National Oceanic and Atmospheric Administration (NOAA) for acquisition, archiving, and dissemination of ocean passive acoustic data._
<!--more-->


# Background

Metadata is data that describes data.  A metadata convention is a systemic set of metadata attributes that have been developed to describe a particular genre or type of data.  This document attempts to create a host metadata list that is necessary to describe passive acoustic datasets from various platforms and sensors from NOAA’s different line offices.  The metadata list will further be used to develop a “machine-readable” metadata template to be tested among passive acoustic data holders and the community.  Hopefully it will eventually be adopted as the NOAA metadata standard for passive acoustic recordings.  The terms “metadata convention” and “metadata standard” are often used interchangeable.  This document details a “convention” which may be followed, as against a “standard” that is more stringent and must be adhered to.  The goal of the eventual development of such a standard will facilitate discovery and exchange of passive acoustic recording data while ensuring its archivability and longevity.


# Summary of Metadata Categories

## Mission / project metadata

This is the metadata that gives a high level description of the overarching initiative (e.g., mission, project, ocean observing system) under which passive acoustic data are collected.

## Platform metadata

This metadata set includes vessel, glider, drifting buoy, and fixed platform (buoy-moored sensor, suspended sensor, and bottom-mounted sensor, etc.).  This metadata describes the platform used to collect passive acoustic data.

## Recording equipment metadata

This metadata include instruments involved in passive acoustic data collection.  The category includes instrumentation, which describes a collection of the instrument package, and each separate component of the instrument package: hydrophone / sensor, pre-amplifier, analogue/digital converter, and recorder.



# Definition of Attributes for Passive Acoustic Recordings Metadata 
<br>

## Category I:  Mission and Project


|	Metadata name	|	Definition	|	Data type \[1\]	|	Unit	|	Authority	|
| ---------- | ---------- | :----------: | :----------: | :---------- |
|	project_ID	|	ID number of mission or project, if exists	|S |		|		|
|	project_name	|	Name of mission or project	|	S	|		|		|
|	project_abstract	|	Free text description of the mission or project, its purpose, scientific objectives and area of operation.  Other instruments and experiments within the mission or project which may or may not relate directly to the passive acoustic data can be included	|	S	|		|		|
|	project_purpose	|	Free text description of the purpose or objective of the project or mission	|		|		|		|
|	data_acknowledgement	|	Any users (including re-packagers) of this data are required to clearly acknowledge the source of the material in this format.  E.g., acknowledge contribution of the datasets	|	S	|		|		|
|	principal_investigator	|	Name of the principal investigator in charge of the mission or project	|	S	|		|		|
|	organizationName	|	Name and address of the organization, facility, or agency where the original data were produced	|	S	|		|	ISO 19115-2:2009(E)	|
|	principal_investigator_position	|	Position and title of the principal investigator	|	S	|		|		|
|	principal_investigator_phone	|	Principal investigator’s phone number	|	S	|		|		|
|	principal_investigator_fax	|	Principal investigator’s facsimile number	|	S	|		|		|
|	principal_investigator_address	|	Principal investigator’s address line	|	S	|		|		|
|	principal_investigator_city	|	Principal investigator’s address city	|	S	|		|		|
|	principal_investigator_state	|	Principal investigator’s state/province or region	|	S	|		|		|
|	principal_investigator_zip	|	Principal investigator’s ZIP or postal code	|	S	|		|		|
|	principal_investigator_country	|	Principal investigator’s country	|	S	|		|		|
|	principal_investigator_email	|	Principal investigator’s e-mail address	|	S	|		|		|
|	contact_instruction	|	Description on how to contact the PI for data	|	S	|		|		|
|	data_update_frequency	|	How often the acoustic data get updated	|	N	|		|		|
|	last_data_update	|	The date when acoustic data were updated	|	N	|		|		|
|	data_update_note	|	Notes for data updates	|	S	|		|		|
|	data_center_contact_name	|	Name of the contact person at the data center	|	S	|		|		|
|	data_center	|	Data center in charge of the data management or party who distributed the resource	|	S	|		|		|
|	data_center_contact_position	|	Position and title of the contact person at the data center	|	S	|		|		|
|	data_center_phone	|	Data center phone number	|	S	|		|		|
|	data_center_fax	|	Data center facsimile number	|	S	|		|		|
|	data_center_address	|	Address line of the data center	|	S	|		|		|
|	data_center_city	|	City where the data center is located	|	S	|		|		|
|	data_center_state	|	State or province where the data center is located	|	S	|		|		|
|	data_center_zip	|	ZIP code or postal code of the data center	|	S	|		|		|
|	data_center_country	|	Country where the data center is located	|	S	|		|		|
|	data_center_e-mail	|	e-mail address of the data center	|	S	|		|		|
|	data_center_website	|	Web site of the data center	|		|		|		|
|	data_center_hours	|	Hours of service of the data center	|	S	|		|		|
|	contact_instruction_data_center	|	Description on how to contact the data center	|	S	|		|		|
|	data_file_name	|	File name of the acoustic data	|		|		|		|
|	data_file_version	|	File version of the acoustic data	|		|		|		|
|	data_type	|	Type of acoustic data (.wav, mp3, etc.)	|		|		|		|
|	compression_technique	|	Acoustic data compression technique, if any	|		|		|		|
|	ambient_noise	|	Place keyword for ambient noise	|		|		|		|
|	animal_sound	|	Place keyword for animal sound	|		|		|		|
|	anthropogenic_noise	|	Place keyword for anthropogenic noise	|		|		|		|
|	Pacific_Ocean	|	Place keyword for Pacific Ocean	|		|		|	GCMD, keywords vs 8.0	|
|	Atlantic_Ocean	|	Place keyword for Atlantic Ocean	|		|		|	GCMD, keywords vs 8.0	|
|	Arctic_Ocean	|	Place keyword for Arctic Ocean	|		|		|	GCMD, keywords vs 8.0	|
|	Indian_Ocean	|	Place keyword for Indian Ocean	|		|		|	GCMD, keywords vs 8.0	|
|	place	|	Keywords for places	|		|		|		|
|	vessel	|	Platform keyword for vessel	|		|		|		|
|	glider	|	Platform keyword for glider	|		|		|	IOOS Platform Vocabulary	|
|	drifting_buoy	|	Platform keyword for drifting buoy	|		|		|	IOOS Platform Vocabulary	|
|	moored_buoy	|	Platform keyword for moored buoy	|		|		|	IOOS Platform Vocabulary	|
|	bottom_mounted	|	Platform keyword for bottom-mounted platform	|		|		|		|
|	platform	|	Keywords for platforms	|		|		|	IOOS Platform Vocabulary	|
|	hydrophone_pressure_sensor	|	Instrument keyword for pressure sensor hydrophone	|		|		|		|
|	hydrophone_vector_sensor	|	Instrument keyword for vector sensor hydrophone	|		|		|		|
|	preamplifier	|	Instrument keyword for pre-amplifier	|		|		|		|
|	AD_converter	|	Instrument keyword for A/D converter	|		|		|		|
|	recorder_analogue	|	Instrument keyword for analogue recorder	|		|		|		|
|	recorder_digital	|	Instrument keyword for digital recorder	|		|		|		|
|	other_signal_conditioning	|	Instrument keyword for other signal conditioning devices	|		|		|		|
|	instrument	|	Keywords for instrument	|		|		|		|
|	NEFSC	|	dataCenter keyword for NEFSC	|		|		|		|
|	SEFSC	|	dataCenter keyword for SEFSC	|		|		|		|
|	NWFSC	|	dataCenter keyword for NWFSC	|		|		|		|
|	SWFSC	|	dataCenter keyword for SWFSC	|		|		|		|
|	AFSC	|	dataCenter keyword for AFSC	|		|		|		|
|	PIFSC	|	dataCenter keyword for PIFSC	|		|		|		|
|	dataCenter	|	Keywords for data centers	|		|		|		|
|	data_restriction	|	Restriction of data distribution	|	S	|		|		|
|	language	|	Language 	|	S	|		|		|
|	project_area_description	|	Description of the project area	|	S	|		|		|
|	project_geospatial_longitude_minimum	|	Westernmost longitude of bounding box.  A value between -180 and 180 decimal degrees East.  Note it is possible for the numeric value of the “geospatial longitude maximum” to be less than the numeric value of the “geospatial longitude minimum.”  In that instance the bounding box will have crossed the 180 degree longitude boundary between West and East.	|	N	|	degrees_east	|	CF	|
|	project_geospatial_longitude_maximum 	|	Easternmost longitude of bounding box.  A value between -180 and 180 decimal degrees East.  Note it is possible for the numeric value of the “geospatial longitude maximum” to be less than the numeric value of the “geospatial longitude minimum.”  In that instance the bounding box will have crossed the 180 degree longitude boundary between West and East.	|	N	|	degrees_east	|	CF	|
|	project_geospatial_latitude_minimum	|	Southernmost latitude of bounding box.  A value between -90 and 90 decimal degrees North	|	N	|	degrees_north	|	CF	|
|	project_geospatial_latitude_maximum	|	Northernmost latitude of bounding box.  A value between -90 and 90 decimal degrees North.	|	N	|	degrees_north	|	CF	|
|	project_start_date	|	Start data of mission or project in ISO 8601 format including local time zone.  For example, a local time of 18:00 on the 24th of October 2008 would be represented as 2008-10-24T08:00:00Z+10 (local).	|	S	|		|		|
|	project_end_date	|	As per mission_start_date	|	S	|		|		|
|	minimum_sensor_depth	|	Minimum sensor depth in m	|		|		|		|
|	maximum_sensor_depth	|	Maximum sensor depth in m	|		|		|		|
|		|		|		|		|		|
|	supplemental_info	|	Additional info	|		|		|		|
										
										
	[1] “S” denotes the entry is a text value, while “N” denotes the entry is a numeric value.									


## Category II:  Platform 

|	Metadata name	|	Definition	|	Data type	|	Units	|
|	------------------------------	|	------------------------------	|	------------------------------	|	------------------------------	|
|	vessel_id	|	ID number of the vessel, if it exists	|	S	|		|
|	acoustic_sampling_start_date	|	Start data of acoustic data collection in ISO 8601 format including local time zone.  For example, a local time of 18:00 on the 24th of October 2008 would be represented as 2008-10-24T08:00:00Z+10 (local).	|		|		|
|	platform_detail	|	Free field provide detailed description of the platform, include tow speed (for towed hydrophone or hydrophone array), number of sensors, array directivity in housing, array geometry, array beamwidth, platform noise signature, platform synchronization, and platform manufacture date, etc. 	|		|		|
|		|		|		|		|
|	glider_name	|	Name of the glider that was used to collect passive acoustic data. 	|	S	|		|
|	glider_id	|	ID number of the glider, if it exists	|	S	|		|
|	acoustic_sampling_start_date	|	Start data of acoustic data collection in ISO 8601 format including local time zone.  For example, a local time of 18:00 on the 24th of October 2008 would be represented as 2008-10-24T08:00:00Z+10 (local).	|		|		|
|	platform_detail	|	Free field provide detailed description of the platform, include number of sensors, array directivity in housing, array geometry, array beamwidth, platform noise signature, platform synchronization, and platform manufacture date, etc. 	|		|		|
|		|		|		|		|
|	drifting_buoy_name	|	Name of the drifting buoy that was used to collect passive acoustic data. 	|	S	|		|
|	drifting_buoy_id	|	ID number of the drifting buoy, if it exists	|	S	|		|
|	acoustic_sampling_start_date	|	Start data of acoustic data collection in ISO 8601 format including local time zone.  For example, a local time of 18:00 on the 24th of October 2008 would be represented as 2008-10-24T08:00:00Z+10 (local).	|		|		|
|	platform_detail	|	Free field provide detailed description of the platform, include tow speed (for towed hydrophone or hydrophone array), number of sensors, array directivity in housing, array geometry, array beamwidth, platform noise signature, platform synchronization, and platform manufacture date, etc. 	|		|		|
|		|		|		|		|
|	moored_buoy_name	|	Name of the moored buoy that was used to collect passive acoustic data. 	|	S	|		|
|	moored_buoy_id	|	ID number of the moored buoy, if it exists	|	S	|		|
|	acoustic_sampling_start_date	|	Start data of acoustic data collection in ISO 8601 format including local time zone.  For example, a local time of 18:00 on the 24th of October 2008 would be represented as 2008-10-24T08:00:00Z+10 (local).	|		|		|
|	platform_detail	|	Free field provide detailed description of the platform, include tow speed (for towed hydrophone or hydrophone array), number of sensors, array directivity in housing, array geometry, array beamwidth, platform noise signature, platform synchronization, and platform manufacture date, etc. 	|		|		|
|		|		|		|		|
|	suspended_platform_name	|	Name of the suspended platform that was used to collect passive acoustic data. 	|	S	|		|
|	suspended_platform_id	|	ID number of the suspended platform, if it exists	|	S	|		|
|	acoustic_sampling_start_date	|	Start data of acoustic data collection in ISO 8601 format including local time zone.  For example, a local time of 18:00 on the 24th of October 2008 would be represented as 2008-10-24T08:00:00Z+10 (local).	|		|		|
|	platform_detail	|	Free field provide detailed description of the platform, include tow speed (for towed hydrophone or hydrophone array), number of sensors, array directivity in housing, array geometry, array beamwidth, platform noise signature, platform synchronization, and platform manufacture date, etc. 	|		|		|
|		|		|		|		|
|	bottom_mounted_platform_name	|	Name of the bottom-mounted platform that was used to collect passive acoustic data. 	|	S	|		|
|	bottom_mounted_platform_id	|	ID number of the bottom-mounted platform, if it exists	|	S	|		|
|	acoustic_sampling_start_date	|	Start data of acoustic data collection in ISO 8601 format including local time zone.  For example, a local time of 18:00 on the 24th of October 2008 would be represented as 2008-10-24T08:00:00Z+10 (local).	|		|		|
|	platform_detail	|	Free field provide detailed description of the platform, include tow speed (for towed hydrophone or hydrophone array), number of sensors, array directivity in housing, array geometry, array beamwidth, platform noise signature, platform synchronization, and platform manufacture date, etc. 	|		|		|


## Category III:  Recording Equipment (sensor, pre-amplifier, A/D converter, additional signal conditioning)

Metadata name	|	Definition	|	Data type	|	Units	|	Authority	|
------------------------------	|	------------------------------	|	:------------------------------:	|	------------------------------	|	------------------------------	|
hydrophone_type	|	pressure sensor or vector sensor	|	S	|		|		|
hydrophone_id	|	ID number of the hydrophone if it exists	|		|		|		|
hydrophone_maker_model	|	Maker or manufacture of the hydrophone that was used to collect passive acoustic data	|		|		|		|
hydrophone_sensitivity	|	Sensitivity of hydrophone and calibration method	|	N	|		|		|
calibration_date	|		|		|		|		|
other_info	|	List noise floor, directivity, and resonance frequency of hydrophone	|	N	|		|		|
	|		|		|		|		|
preamplifier_id	|	ID number of the pre-amplifier if it exists	|		|		|		|
preamplifier_maker_model	|	Maker or manufacture of the preamplifier that was used to collect passive acoustic data	|		|		|		|
preamplifier_gain	|	For pre-amplifier, A/D converter, and signal conditioning only	|	N	|		|		|
other_info	|	Other info related to the pre-amplifier, such as noise floor, low- and high-pass filter specification, etc., if available.	|		|		|		|
	|		|		|		|		|
AD_converter_id	|	ID number of the AD converter if it exists	|		|		|		|
AD_converter_maker_model	|		|		|		|		|
sample_rate	|		|		|		|		|
other_info	|	Additional info related to the AD converter, such as gain, noise floor, and bit rate, etc.	|		|		|		|
	|		|		|		|		|
recorder_type	|	analogue vs. digital recorder	|	S	|		|		|
recorder_id	|	ID number of the recorder if it exists	|		|		|		|
recorder_maker_model	|	Maker or manufacture of the recorder that was used to collect passive acoustic data	|		|		|		|
recorder_gain	|	Signal gain of the recorder	|	N	|		|		|
other_info	|	Additional info related to the recorder, such as noise floor, etc.	|		|		|		|
	|		|		|		|		|
additional_signal_con_type	|	Types of additional signal conditioning device, if available	|	S	|		|		|
device_id	|	ID number of the instrument if it exists	|		|		|		|
device_maker_model	|	Maker or manufacture of the device that was used to collect passive acoustic data	|		|		|		|
device_function	|	Functionality of the device	|		|		|		|
other_info	|	Additional info related to the device, such as signal gain, noise floor, etc.	|	N	|		|		|


# ISO 19115  XML Template for NOAA Passive Acoustic Recordings


```

<!-- <gmd:metadataStandardName>
     <gco:CharacterString>METADATA CONVENTION FOR IOOS PASSIVE ACOUSTIC RECORDINGS</gco:CharacterString>
     version 1.0 2013/08/13 Shane Guan (NMFS, Silver Spring, MD), Hassan Moustahfid (US IOOS, Silver Spring, MD) and Anna Milan (NOAA NGDC, Boulder, CO), Jacqueline Mize (NOAA NCDDC, Stennis, MS)-->

<?xml-stylesheet type="text/css" href="http://www.ngdc.noaa.gov/metadata/published/views/ISO.css"?>
<gmi:MI_Metadata xmlns:gmi="http://www.isotc211.org/2005/gmi" xmlns:gmd="http://www.isotc211.org/2005/gmd" xmlns:gco="http://www.isotc211.org/2005/gco" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:gml="http://www.opengis.net/gml/3.2" xmlns:srv="http://www.isotc211.org/2005/srv" xmlns:gmx="http://www.isotc211.org/2005/gmx" xmlns:gss="http://www.isotc211.org/2005/gss" xmlns:gsr="http://www.isotc211.org/2005/gsr" xmlns:gts="http://www.isotc211.org/2005/gts" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.isotc211.org/2005/gmi http://www.ngdc.noaa.gov/metadata/published/xsd/schema.xsd">
  <gmd:fileIdentifier>
    <gco:CharacterString>project_ID</gco:CharacterString>
  </gmd:fileIdentifier>
  <gmd:language>
    <gco:CharacterString>eng; USA</gco:CharacterString>
  </gmd:language>
  <gmd:contact>
    <gmd:CI_ResponsibleParty>
      <gmd:individualName>
        <gco:CharacterString>template</gco:CharacterString>
      </gmd:individualName>
      <gmd:organisationName>
        <gco:CharacterString>template</gco:CharacterString>
      </gmd:organisationName>
      <gmd:positionName>
        <gco:CharacterString>template</gco:CharacterString>
      </gmd:positionName>
      <gmd:contactInfo>
        <gmd:CI_Contact>
          <gmd:phone>
            <gmd:CI_Telephone>
              <gmd:voice>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:voice>
              <gmd:facsimile>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:facsimile>
            </gmd:CI_Telephone>
          </gmd:phone>
          <gmd:address>
            <gmd:CI_Address>
              <gmd:deliveryPoint>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:deliveryPoint>
              <gmd:city>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:city>
              <gmd:administrativeArea>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:administrativeArea>
              <gmd:postalCode>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:postalCode>
              <gmd:country>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:country>
              <gmd:electronicMailAddress>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:electronicMailAddress>
            </gmd:CI_Address>
          </gmd:address>
          <gmd:hoursOfService>
            <gco:CharacterString>template</gco:CharacterString>
          </gmd:hoursOfService>
          <gmd:contactInstructions>
            <gco:CharacterString>template</gco:CharacterString>
          </gmd:contactInstructions>
        </gmd:CI_Contact>
      </gmd:contactInfo>
      <gmd:role>
        <gmd:CI_RoleCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#CI_RoleCode" codeListValue="code">code</gmd:CI_RoleCode>
      </gmd:role>
    </gmd:CI_ResponsibleParty>
  </gmd:contact>
  <gmd:dateStamp>
    <gco:Date>2013-08-28</gco:Date>
  </gmd:dateStamp>
  <gmd:metadataStandardName>
    <gco:CharacterString>ISO 19115-2 Geographic Information - Metadata - Part 2: Extensions for Imagery and Gridded Data</gco:CharacterString>
  </gmd:metadataStandardName>
  <gmd:metadataStandardVersion>
    <gco:CharacterString>ISO 19115-2:2009(E)</gco:CharacterString>
  </gmd:metadataStandardVersion>
<!--insert spatial information if needed as example below details-->
<gmd:referenceSystemInfo>
<gmd:MD_ReferenceSystem uuid="895cc120-95ed-11e0-aa80-0800200c9a66">
    <gmd:referenceSystemIdentifier>
      <gmd:RS_Identifier>
        <gmd:authority>
          <gmd:CI_Citation>
            <gmd:title>
              <gco:CharacterString>WGS 84 / World Mercator</gco:CharacterString>
            </gmd:title>
            <gmd:date>
              <gmd:CI_Date>
                <gmd:date>
                  <gco:Date>2006-06-02</gco:Date>
                </gmd:date>
                <gmd:dateType>
                  <gmd:CI_DateTypeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#CI_DateTypeCode" codeListValue="revision">revision</gmd:CI_DateTypeCode>
                </gmd:dateType>
              </gmd:CI_Date>
            </gmd:date>
            <gmd:citedResponsibleParty>
              <gmd:CI_ResponsibleParty>
                <gmd:contactInfo>
                  <gmd:CI_Contact>
                    <gmd:onlineResource>
                      <gmd:CI_OnlineResource>
                        <gmd:linkage>
                          <gmd:URL>
                            http://www.epsg-registry.org/export.htm?gml=urn:ogc:def:crs:EPSG::3395
                          </gmd:URL>
                        </gmd:linkage>
                      </gmd:CI_OnlineResource>
                    </gmd:onlineResource>
                  </gmd:CI_Contact>
                </gmd:contactInfo>
                <gmd:role>
                  <gmd:CI_RoleCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#CI_RoleCode" codeListValue="resourceProvider" codeSpace="001">resourceProvider</gmd:CI_RoleCode>
                </gmd:role>
              </gmd:CI_ResponsibleParty>
            </gmd:citedResponsibleParty>
          </gmd:CI_Citation>
        </gmd:authority>
        <gmd:code>
          <gco:CharacterString>urn:ogc:def:crs:EPSG::3395</gco:CharacterString>
        </gmd:code>
      </gmd:RS_Identifier>
    </gmd:referenceSystemIdentifier>
  </gmd:MD_ReferenceSystem>
</gmd:referenceSystemInfo>
  <gmd:identificationInfo>
    <gmd:MD_DataIdentification>
      <gmd:citation>
        <gmd:CI_Citation>
          <gmd:title>
            <gco:CharacterString>project_name</gco:CharacterString>
          </gmd:title>
          <gmd:date>
            <gmd:CI_Date>
              <gmd:date>
                <gco:Date>9999-01-01</gco:Date>
              </gmd:date>
              <gmd:dateType>
                <gmd:CI_DateTypeCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#CI_DateTypeCode" codeListValue="creation">creation</gmd:CI_DateTypeCode>
              </gmd:dateType>
            </gmd:CI_Date>
          </gmd:date>
          <!-- last_data_update -->
          <gmd:date>
            <gmd:CI_Date>
              <gmd:date>
                <gco:Date>9999-01-01</gco:Date>
              </gmd:date>
              <gmd:dateType>
                <gmd:CI_DateTypeCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#CI_DateTypeCode" codeListValue="revision">revision</gmd:CI_DateTypeCode>
              </gmd:dateType>
            </gmd:CI_Date>
          </gmd:date>
        </gmd:CI_Citation>
      </gmd:citation>
      <gmd:abstract>
        <gco:CharacterString>project_abstract</gco:CharacterString>
      </gmd:abstract>
      <gmd:purpose>
        <gco:CharacterString>project_purpose</gco:CharacterString>
      </gmd:purpose>
      <gmd:credit>
        <gco:CharacterString>data_acknowledgement</gco:CharacterString>
      </gmd:credit>
      <gmd:pointOfContact>
        <gmd:CI_ResponsibleParty>
          <gmd:individualName>
            <gco:CharacterString>principal_investigator</gco:CharacterString>
          </gmd:individualName>
          <gmd:organisationName>
            <gco:CharacterString>organization</gco:CharacterString>
          </gmd:organisationName>
          <gmd:positionName>
            <gco:CharacterString>principal_investigator_position</gco:CharacterString>
          </gmd:positionName>
          <gmd:contactInfo>
            <gmd:CI_Contact>
              <gmd:phone>
                <gmd:CI_Telephone>
                  <gmd:voice>
                    <gco:CharacterString>principal_investigator_phone</gco:CharacterString>
                  </gmd:voice>
                  <gmd:facsimile>
                    <gco:CharacterString>principal_investigator_fax</gco:CharacterString>
                  </gmd:facsimile>
                </gmd:CI_Telephone>
              </gmd:phone>
              <gmd:address>
                <gmd:CI_Address>
                  <gmd:city>
                    <gco:CharacterString>principal_investigator_city</gco:CharacterString>
                  </gmd:city>
                  <gmd:administrativeArea>
                    <gco:CharacterString>principal_investigator_state</gco:CharacterString>
                  </gmd:administrativeArea>
                  <gmd:postalCode>
                    <gco:CharacterString>principal_investigator_zip</gco:CharacterString>
                  </gmd:postalCode>
                  <gmd:country>
                    <gco:CharacterString>principal_investigator_country</gco:CharacterString>
                  </gmd:country>
                  <gmd:electronicMailAddress>
                    <gco:CharacterString>principal_investigator_address</gco:CharacterString>
                  </gmd:electronicMailAddress>
                </gmd:CI_Address>
              </gmd:address>
              <gmd:hoursOfService>
                <gco:CharacterString>template</gco:CharacterString>
              </gmd:hoursOfService>
              <gmd:contactInstructions>
                <gco:CharacterString>contact_instruction</gco:CharacterString>
              </gmd:contactInstructions>
            </gmd:CI_Contact>
          </gmd:contactInfo>
          <gmd:role>
            <gmd:CI_RoleCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#CI_RoleCode" codeListValue="principalInvestigator">principalInvestigator</gmd:CI_RoleCode>
          </gmd:role>
        </gmd:CI_ResponsibleParty>
      </gmd:pointOfContact>
      <gmd:resourceMaintenance>
        <gmd:MD_MaintenanceInformation>
          <gmd:maintenanceAndUpdateFrequency>
            <!-- data_update_frequency will need to conform to the codelist values -->
            <gmd:MD_MaintenanceFrequencyCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#MD_MaintenanceFrequencyCode" codeListValue="code">data_update_frequency</gmd:MD_MaintenanceFrequencyCode>
          </gmd:maintenanceAndUpdateFrequency>
          <gmd:dateOfNextUpdate>
            <gco:Date>9999-01-01</gco:Date>
          </gmd:dateOfNextUpdate>
          <gmd:maintenanceNote>
            <gco:CharacterString>data_update_note</gco:CharacterString>
          </gmd:maintenanceNote>
          <gmd:contact>
            <gmd:CI_ResponsibleParty>
              <gmd:individualName>
                <gco:CharacterString>data_center_contact_name</gco:CharacterString>
              </gmd:individualName>
              <gmd:organisationName>
                <gco:CharacterString>data_center</gco:CharacterString>
              </gmd:organisationName>
              <gmd:positionName>
                <gco:CharacterString>data_center_contact_position</gco:CharacterString>
              </gmd:positionName>
              <gmd:contactInfo>
                <gmd:CI_Contact>
                  <gmd:phone>
                    <gmd:CI_Telephone>
                      <gmd:voice>
                        <gco:CharacterString>data_center_phone</gco:CharacterString>
                      </gmd:voice>
                      <gmd:facsimile>
                        <gco:CharacterString>data_center_fax</gco:CharacterString>
                      </gmd:facsimile>
                    </gmd:CI_Telephone>
                  </gmd:phone>
                  <gmd:address>
                    <gmd:CI_Address>
                      <gmd:deliveryPoint>
                        <gco:CharacterString>template</gco:CharacterString>
                      </gmd:deliveryPoint>
                      <gmd:city>
                        <gco:CharacterString>data_center_city</gco:CharacterString>
                      </gmd:city>
                      <gmd:administrativeArea>
                        <gco:CharacterString>data_center_state</gco:CharacterString>
                      </gmd:administrativeArea>
                      <gmd:postalCode>
                        <gco:CharacterString>data_center_zip</gco:CharacterString>
                      </gmd:postalCode>
                      <gmd:country>
                        <gco:CharacterString>data_center_country</gco:CharacterString>
                      </gmd:country>
                      <gmd:electronicMailAddress>
                        <gco:CharacterString>data_center_address</gco:CharacterString>
                      </gmd:electronicMailAddress>
                    </gmd:CI_Address>
                  </gmd:address>
                  <gmd:onlineResource>
                    <gmd:CI_OnlineResource>
                      <gmd:linkage>
                        <gmd:URL>data_center_website</gmd:URL>
                      </gmd:linkage>
                    </gmd:CI_OnlineResource>
                  </gmd:onlineResource>
                  <gmd:hoursOfService>
                    <gco:CharacterString>data_center_hours</gco:CharacterString>
                  </gmd:hoursOfService>
                  <gmd:contactInstructions>
                    <gco:CharacterString>contact_instruction_data_center</gco:CharacterString>
                  </gmd:contactInstructions>
                </gmd:CI_Contact>
              </gmd:contactInfo>
              <gmd:role>
                <gmd:CI_RoleCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#CI_RoleCode" codeListValue="code">code</gmd:CI_RoleCode>
              </gmd:role>
            </gmd:CI_ResponsibleParty>
          </gmd:contact>
        </gmd:MD_MaintenanceInformation>
      </gmd:resourceMaintenance>
      <gmd:resourceFormat>
        <gmd:MD_Format>
          <gmd:name>
            <gco:CharacterString>data_type</gco:CharacterString>
          </gmd:name>
          <gmd:version>
            <gco:CharacterString>data_file_version</gco:CharacterString>
          </gmd:version>
          <gmd:specification>
            <gco:CharacterString>data_file_name</gco:CharacterString>
          </gmd:specification>
          <gmd:fileDecompressionTechnique>
            <gco:CharacterString>compression_technique</gco:CharacterString>
          </gmd:fileDecompressionTechnique>
        </gmd:MD_Format>
      </gmd:resourceFormat>
      <!-- ARE THERE CONTROLLED VOCABULARIES TO REPRESENT THESE VALUES? -->
      <gmd:descriptiveKeywords>
        <gmd:MD_Keywords>
          <gmd:keyword>
            <gco:CharacterString>ambient_noise</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>animal_sound</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>anthropogenic_noise</gco:CharacterString>
          </gmd:keyword>
          <!--add type of keyword-->
          <gmd:type>
			  <gmd:MD_KeywordTypeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#MD_KeywordTypeCode" codeListValue="theme" codeSpace="005">theme</gmd:MD_KeywordTypeCode>
		</gmd:type>
          <!--add name of thesaurus that these values come from...if none or user defined use citation as below-->
          <gmd:thesaurusName>
			  <gmd:CI_Citation>
				<gmd:title>
					<gco:CharacterString>None</gco:CharacterString>
				</gmd:title>
				<gmd:date gco:nilReason="unknown"/>
			 </gmd:CI_Citation>
		  </gmd:thesaurusName>
        </gmd:MD_Keywords>
      </gmd:descriptiveKeywords>
      <!-- HOW ARE THESE VALUES DETERMINED? -->
      <gmd:descriptiveKeywords>
        <gmd:MD_Keywords>
          <gmd:keyword>
            <!-- GET A LIST OF LOCATION KEYWORDS FROM GCMD -->
            <gco:CharacterString>Pacific_Ocean</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>Atlantic_Ocean</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>Arctic_Ocean</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>Indian_Ocean</gco:CharacterString>
          </gmd:keyword>
          <gmd:type>
            <gmd:MD_KeywordTypeCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#MD_KeywordTypeCode" codeListValue="place">place</gmd:MD_KeywordTypeCode>
          </gmd:type>
        </gmd:MD_Keywords>
      </gmd:descriptiveKeywords>
      <!-- WOULD IT BE ALL OF THESE VALUES OR SOME? -->
      <gmd:descriptiveKeywords>
        <gmd:MD_Keywords>
          <gmd:keyword>
            <gco:CharacterString>vessel</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>glider</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>drifting_buoy</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>moored_buoy</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>bottom_mounted</gco:CharacterString>
          </gmd:keyword>
          <gmd:type>
            <gmd:MD_KeywordTypeCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#MD_KeywordTypeCode" codeListValue="platform">platform</gmd:MD_KeywordTypeCode>
          </gmd:type>
        </gmd:MD_Keywords>
      </gmd:descriptiveKeywords>
      <gmd:descriptiveKeywords>
        <gmd:MD_Keywords>
          <gmd:keyword>
            <gco:CharacterString>hydrophone_pressure_sensor</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>hydrophone_vector_sensor</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>preamplifier</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>AD_converter</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>recorder_analogue</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>recorder_digital</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>other_signal_conditioning</gco:CharacterString>
          </gmd:keyword>
          <gmd:type>
            <gmd:MD_KeywordTypeCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#MD_KeywordTypeCode" codeListValue="instrument">instrument</gmd:MD_KeywordTypeCode>
          </gmd:type>

        </gmd:MD_Keywords>
      </gmd:descriptiveKeywords>

      <gmd:descriptiveKeywords>
        <gmd:MD_Keywords>
          <gmd:keyword>
            <gco:CharacterString>NOAA Northeast Fisheries Science Center</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>NOAA Southeast Fisheries Science Center</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>NOAA Northwest Fisheries Science Center</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>NOAA Southwest Fisheries Science Center</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>NOAA Alaska Fisheries Science Center</gco:CharacterString>
          </gmd:keyword>
          <gmd:keyword>
            <gco:CharacterString>NOAA Pacific Islands Fisheries Science Center</gco:CharacterString>
          </gmd:keyword>
          <gmd:type>
            <gmd:MD_KeywordTypeCode codeList="http://www.ngdc.noaa.gov/metadata/published/xsd/schema/resources/Codelist/gmxCodelists.xml#MD_KeywordTypeCode" codeListValue="dataCenter">dataCenter</gmd:MD_KeywordTypeCode>
          </gmd:type>
        </gmd:MD_Keywords>
      </gmd:descriptiveKeywords>
      <gmd:resourceConstraints>
        <gmd:MD_Constraints>
          <gmd:useLimitation>
            <gco:CharacterString>data_restriction</gco:CharacterString>
          </gmd:useLimitation>
        </gmd:MD_Constraints>
      </gmd:resourceConstraints>
      <gmd:language>
        <gco:CharacterString>eng; USA</gco:CharacterString>
      </gmd:language>      

      <gmd:topicCategory>
        <gmd:MD_TopicCategoryCode>oceans</gmd:MD_TopicCategoryCode>
      </gmd:topicCategory>

      <gmd:extent>
        <gmd:EX_Extent id="boundingExtent">
          <gmd:description>
            <gco:CharacterString>project_area_description</gco:CharacterString>
          </gmd:description>
          <gmd:geographicElement>
            <gmd:EX_GeographicBoundingBox>
              <gmd:westBoundLongitude>

                <gco:Decimal>-180</gco:Decimal>
              </gmd:westBoundLongitude>
              <gmd:eastBoundLongitude>

                <gco:Decimal>180</gco:Decimal>
              </gmd:eastBoundLongitude>
              <gmd:southBoundLatitude>

                <gco:Decimal>-90</gco:Decimal>
              </gmd:southBoundLatitude>
              <gmd:northBoundLatitude>

                <gco:Decimal>90</gco:Decimal>
              </gmd:northBoundLatitude>
            </gmd:EX_GeographicBoundingBox>
          </gmd:geographicElement>
          <gmd:temporalElement>
            <gmd:EX_TemporalExtent id="boundingTemporalExtent">
              <gmd:extent>
                <gml:TimePeriod gml:id="ID072">
                  <!--                 project_start_date-->
                  <gml:beginPosition>9999-01-01</gml:beginPosition>
                  <!--                  project_end_date-->
                  <gml:endPosition>9999-01-01</gml:endPosition>
                </gml:TimePeriod>
              </gmd:extent>
            </gmd:EX_TemporalExtent>
          </gmd:temporalElement>
          <gmd:verticalElement>
            <gmd:EX_VerticalExtent>
              <gmd:minimumValue>
                <!--                <gco:Real>minimum_sensor_depth</gco:Real>-->
                <gco:Real>99</gco:Real>
                <!--                <gco:Real>minimum_sensor_depth</gco:Real>-->
              </gmd:minimumValue>
              <gmd:maximumValue>
                <!--                <gco:Real>maximum_sensor_depth</gco:Real>-->
                <gco:Real>99</gco:Real>
                <!--                <gco:Real>maximum_sensor_depth</gco:Real>-->
              </gmd:maximumValue>
              <!-- WHAT ARE THE VERTICAL REFERENCES USUALLY USED? WILL THIS INFO BE AVAILABLE TO POPULATE THE METADATA RECORD? -->
              <gmd:verticalCRS>
                <gml:VerticalCRS gml:id="ID384">
                  <gml:description>template</gml:description>
                  <gml:identifier codeSpace="template">template</gml:identifier>
                  <gml:name>template</gml:name>
                  <gml:remarks>template</gml:remarks>
                  <gml:scope>template</gml:scope>
                  <gml:verticalCS>
                    <gml:VerticalCS gml:id="ID058">
                      <gml:description>template</gml:description>
                      <gml:identifier codeSpace="template">template</gml:identifier>
                      <gml:name>template</gml:name>
                      <gml:remarks>template</gml:remarks>
                      <gml:axis>
                        <gml:CoordinateSystemAxis uom="template" gml:id="ID060">
                          <gml:description>template</gml:description>
                          <gml:identifier codeSpace="template">template</gml:identifier>
                          <gml:name>template</gml:name>
                          <gml:remarks>template</gml:remarks>
                          <gml:axisAbbrev>template</gml:axisAbbrev>
                          <gml:axisDirection codeSpace="template">template</gml:axisDirection>
                          <gml:minimumValue>99</gml:minimumValue>
                          <gml:maximumValue>99</gml:maximumValue>
                          <gml:rangeMeaning codeSpace="template">template</gml:rangeMeaning>
                        </gml:CoordinateSystemAxis>
                      </gml:axis>
                    </gml:VerticalCS>
                  </gml:verticalCS>
                  <gml:verticalDatum>
                    <gml:VerticalDatum gml:id="ID062">
                      <gml:metaDataProperty>
                        <gml:GenericMetaData/>
                      </gml:metaDataProperty>
                      <!--<gml:description>template</gml:description>-->
                      <!--<gml:descriptionReference/>-->
                      <gml:identifier codeSpace="template">template</gml:identifier>
                      <!--<gml:name>template</gml:name>-->
                      <!--<gml:remarks>template</gml:remarks>-->
                      <gml:scope>template</gml:scope>
                    </gml:VerticalDatum>
                  </gml:verticalDatum>
                </gml:VerticalCRS>
              </gmd:verticalCRS>
            </gmd:EX_VerticalExtent>
          </gmd:verticalElement>
        </gmd:EX_Extent>
      </gmd:extent>
      <gmd:supplementalInformation>
        <gco:CharacterString>supplemental_info</gco:CharacterString>
      </gmd:supplementalInformation>
    </gmd:MD_DataIdentification>
  </gmd:identificationInfo>
  <gmi:acquisitionInformation>
    <gmi:MI_AcquisitionInformation>
      <!-- VESSEL -->
      <gmi:platform>
        <!--      vessel_name,acoustic_sampling_start_date-->
        <gmi:MI_Platform>
          <gmi:identifier>
            <gmd:MD_Identifier>
              <gmd:code>
                <gco:CharacterString>vessel_id</gco:CharacterString>
              </gmd:code>
            </gmd:MD_Identifier>
          </gmi:identifier>
          <gmi:description>
            <gco:CharacterString>platform_detail</gco:CharacterString>
          </gmi:description>
          <!-- HYDROPHONE -->
          <gmi:instrument>
            <!-- TO DO: PUT THIS INFO IN CONTENTINFO SECTION: hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>hydrophone_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>hydrophone_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- PREAMPLIFIER -->
          <gmi:instrument>
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>preamplifier_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>preamplifier_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>preamplifier_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- CONVERTER -->
          <gmi:instrument>
            <!-- AD_converter_maker_model,sample_rate,AD_converter_id,other_info-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>AD_converter_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>AD_converter_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>sample_rate,other_info </gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- RECORDER -->
          <gmi:instrument>
            <!--recorder_maker_model-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>recorder_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>recorder_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>recorder_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- DEVICE -->
          <gmi:instrument>
            <!-- 
              device_maker_model
              device_function              
              other_info
              additional_signal_con_type
            -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>device_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type/>
              <gmi:description>
                <gco:CharacterString>device_maker_model, device_function, other_info, additional_signal_con_type</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>

        </gmi:MI_Platform>
      </gmi:platform>
      <!-- GLIDER -->
      <gmi:platform>
        <!-- 
          glider_name,
          acoustic_sampling_start_date,
        -->
        <gmi:MI_Platform>
          <gmi:identifier>
            <gmd:MD_Identifier>
              <gmd:code>
                <gco:CharacterString>glider_id</gco:CharacterString>
              </gmd:code>
            </gmd:MD_Identifier>
          </gmi:identifier>
          <gmi:description>
            <gco:CharacterString>platform_detail</gco:CharacterString>
          </gmi:description>
          <!-- HYDROPHONE -->
          <gmi:instrument>
            <!-- TO DO: PUT THIS INFO IN CONTENTINFO SECTION: hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>hydrophone_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>hydrophone_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- PREAMPLIFIER -->
          <gmi:instrument>
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>preamplifier_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>preamplifier_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>preamplifier_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- CONVERTER -->
          <gmi:instrument>
            <!-- AD_converter_maker_model,sample_rate,AD_converter_id,other_info-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>AD_converter_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>AD_converter_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>sample_rate,other_info </gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- RECORDER -->
          <gmi:instrument>
            <!--recorder_maker_model-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>recorder_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>recorder_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>recorder_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- DEVICE -->
          <gmi:instrument>
            <!-- 
              device_maker_model
              device_function              
              other_info
              additional_signal_con_type
            -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>device_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type/>
              <gmi:description>
                <gco:CharacterString>device_maker_model, device_function, other_info, additional_signal_con_type</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
        </gmi:MI_Platform>
      </gmi:platform>
      <!-- DRIFITING BUOY -->
      <gmi:platform>
        <!--drifting_buoy_name, 
        acoustic_sampling_start_date-->
        <gmi:MI_Platform>
          <gmi:identifier>
            <gmd:MD_Identifier>
              <gmd:code>
                <gco:CharacterString>drifting_buoy_id</gco:CharacterString>
              </gmd:code>
            </gmd:MD_Identifier>
          </gmi:identifier>
          <gmi:description>
            <gco:CharacterString>platform_detail</gco:CharacterString>
          </gmi:description>
          <!-- HYDROPHONE -->
          <gmi:instrument>
            <!-- TO DO: PUT THIS INFO IN CONTENTINFO SECTION: hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>hydrophone_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>hydrophone_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- PREAMPLIFIER -->
          <gmi:instrument>
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>preamplifier_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>preamplifier_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>preamplifier_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- CONVERTER -->
          <gmi:instrument>
            <!-- AD_converter_maker_model,sample_rate,AD_converter_id,other_info-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>AD_converter_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>AD_converter_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>sample_rate,other_info </gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- RECORDER -->
          <gmi:instrument>
            <!--recorder_maker_model-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>recorder_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>recorder_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>recorder_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- DEVICE -->
          <gmi:instrument>
            <!-- 
              device_maker_model
              device_function              
              other_info
              additional_signal_con_type
            -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>device_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type/>
              <gmi:description>
                <gco:CharacterString>device_maker_model, device_function, other_info, additional_signal_con_type</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
        </gmi:MI_Platform>
      </gmi:platform>
      <gmi:platform>
        <!--moored_buoy_name
        acoustic_sampling_start_date-->
        <gmi:MI_Platform>
          <gmi:identifier>
            <gmd:MD_Identifier>
              <gmd:code>
                <gco:CharacterString>moored_buoy_id</gco:CharacterString>
              </gmd:code>
            </gmd:MD_Identifier>
          </gmi:identifier>
          <gmi:description>
            <gco:CharacterString>platform_detail</gco:CharacterString>
          </gmi:description>
          <!-- HYDROPHONE -->
          <gmi:instrument>
            <!-- TO DO: PUT THIS INFO IN CONTENTINFO SECTION: hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>hydrophone_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>hydrophone_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- PREAMPLIFIER -->
          <gmi:instrument>
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>preamplifier_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>preamplifier_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>preamplifier_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- CONVERTER -->
          <gmi:instrument>
            <!-- AD_converter_maker_model,sample_rate,AD_converter_id,other_info-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>AD_converter_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>AD_converter_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>sample_rate,other_info </gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- RECORDER -->
          <gmi:instrument>
            <!--recorder_maker_model-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>recorder_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>recorder_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>recorder_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- DEVICE -->
          <gmi:instrument>
            <!-- 
              device_maker_model
              device_function              
              other_info
              additional_signal_con_type
            -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>device_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type/>
              <gmi:description>
                <gco:CharacterString>device_maker_model, device_function, other_info, additional_signal_con_type</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
        </gmi:MI_Platform>
      </gmi:platform>
      <gmi:platform>
        <!--suspended_platform_name,acoustic_sampling_start_date-->
        <gmi:MI_Platform>
          <gmi:identifier>
            <gmd:MD_Identifier>
              <gmd:code>
                <gco:CharacterString>suspended_platform_id</gco:CharacterString>
              </gmd:code>
            </gmd:MD_Identifier>
          </gmi:identifier>
          <gmi:description>
            <gco:CharacterString>platform_detail</gco:CharacterString>
          </gmi:description>
          <!-- HYDROPHONE -->
          <gmi:instrument>
            <!-- TO DO: PUT THIS INFO IN CONTENTINFO SECTION: hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>hydrophone_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>hydrophone_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- PREAMPLIFIER -->
          <gmi:instrument>
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>preamplifier_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>preamplifier_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>preamplifier_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- CONVERTER -->
          <gmi:instrument>
            <!-- AD_converter_maker_model,sample_rate,AD_converter_id,other_info-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>AD_converter_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>AD_converter_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>sample_rate,other_info </gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- RECORDER -->
          <gmi:instrument>
            <!--recorder_maker_model-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>recorder_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>recorder_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>recorder_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- DEVICE -->
          <gmi:instrument>
            <!-- 
              device_maker_model
              device_function              
              other_info
              additional_signal_con_type
            -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>device_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type/>
              <gmi:description>
                <gco:CharacterString>device_maker_model, device_function, other_info, additional_signal_con_type</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
        </gmi:MI_Platform>
      </gmi:platform>
      <gmi:platform>
        <!--bottom_mounted_platform_name
        acoustic_sampling_start_date-->
        <gmi:MI_Platform>
          <gmi:identifier>
            <gmd:MD_Identifier>
              <gmd:code>
                <gco:CharacterString>bottom_mounted_platform_id</gco:CharacterString>
              </gmd:code>
            </gmd:MD_Identifier>
          </gmi:identifier>
          <gmi:description>
            <gco:CharacterString>platform_detail</gco:CharacterString>
          </gmi:description>
          <!-- HYDROPHONE -->
          <gmi:instrument>
            <!-- TO DO: PUT THIS INFO IN CONTENTINFO SECTION: hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>hydrophone_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>hydrophone_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>hydrophone_maker_model,calibration_date,hydrophone_sensitivity,hydrophone_id,other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- PREAMPLIFIER -->
          <gmi:instrument>
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>preamplifier_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>preamplifier_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>preamplifier_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- CONVERTER -->
          <gmi:instrument>
            <!-- AD_converter_maker_model,sample_rate,AD_converter_id,other_info-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>AD_converter_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>AD_converter_maker_model</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>sample_rate,other_info </gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- RECORDER -->
          <gmi:instrument>
            <!--recorder_maker_model-->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>recorder_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type>
                <gco:CharacterString>recorder_type</gco:CharacterString>
              </gmi:type>
              <gmi:description>
                <gco:CharacterString>recorder_gain, other_info</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
          <!-- DEVICE -->
          <gmi:instrument>
            <!-- 
              device_maker_model
              device_function              
              other_info
              additional_signal_con_type
            -->
            <gmi:MI_Instrument>
              <gmi:identifier>
                <gmd:MD_Identifier>
                  <gmd:code>
                    <gco:CharacterString>device_id</gco:CharacterString>
                  </gmd:code>
                </gmd:MD_Identifier>
              </gmi:identifier>
              <gmi:type/>
              <gmi:description>
                <gco:CharacterString>device_maker_model, device_function, other_info, additional_signal_con_type</gco:CharacterString>
              </gmi:description>
            </gmi:MI_Instrument>
          </gmi:instrument>
        </gmi:MI_Platform>
      </gmi:platform>
    </gmi:MI_AcquisitionInformation>
  </gmi:acquisitionInformation>
</gmi:MI_Metadata>

```


# REFERENCE INFORMATION

## Contribution

| Name  | Association  |
|:---|:---|
| **Shane Guan** | NOAA/National Marine Fisheries Service, Office of Protected Resources Silver Spring, MD, USA |
|[**Hassan Moustahfid**](Hassan.Moustahfid@noaa.gov) | NOAA, U.S. Integrated Ocean Observing System Program Office (**corresponding author**) |
| **Anna Milan** | NOAA, National Geophysical Data Center, Boulder, CO, USA |
| **Jacqueline Mize** | NOAA, National Coastal Data Development Center, Stennis, MS, USA |



## Validation

| Name  | Association  |
|:---|:---|
|**Zdenka Willis** | Director of U.S. Integrated Ocean Observing System Program Office |

## Revisions

| Date |  Version | Notes 
| :------ | :------------:| :---------                                                      
|August 2014 | 1.0 | 
                                                           
 
## Acknowledgments

Special thanks go to Sofia VanParijs (NOAA, NEFSC), Jason Gedamke (NOAA, NMFS OS&T) for comments and suggestions that considerably improved this document content.  We also appreciate the support from Jolie Harrison (NOAA, NMFS OPR), Zdenka Willis (US IOOS), Charlie Alexander (IOOS), and Dr. Christopher Fox (NGDC) for supporting this joint effort.

## Endorsement Disclaimer

Mention of a commercial company or product does not constitute an endorsement by NOAA. Use of information from this publication for publicity or advertising purposes concerning proprietary products or the tests of such products is not authorized.

## Citation

- [**The PDF version of this document**](https://github.com/abirger/animal-telemetry/blob/master/doc/noaa_passive_acoustic_metadata_convention_v1.0-FF.pdf?raw=true)



&nbsp; <br>
