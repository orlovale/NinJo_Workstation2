---
title: Technical Information
menus: technical
---


NinJo was developed by a consortium of National Meteorological Services with assistance of experienced IT companies.

The involvement of the different partners in the development of the system ensures both its broad applicability and its continued maintenance. It also ensures that recommendations and requirements of users, configurators, administrators and IT specialists are considered in the development process. As a result, NinJo already encompasses a wide range of the functionalities expected from a workstation system used in operational meteorology. Furthermore, customer-specific functionalities can easily be incorporated into the system.

Distributed offices with central servers in the headquarters are common practice for the Consortium Members, who also share the need for a comprehensive workstation capable of

- visualizing meteorological and oceanographic data from various sources and in various formats,
- producing standard and customized products, and
- editing the data and products.

**General Architecture**

NinJo is a client-server system built using an extremely modular and scalable design. On the client’s side there is the interactive NinJo application, which is installed locally on the user's computer. Batch applications can be implemented on the server as well as on the client’s side. All other data is managed by the relevant server entities and administered centrally. The import/export modules for the different data types as well as decoding of the incoming data also run at the server level.

Optional integration of the GloBUS decoding system allows further optimisation to be achieved. GloBUS was developed on behalf of the German Meteorological Service (DWD) for processing incoming data.

NinJo is open for future developments. The system can easily be extended by further layers and applications according to user-specific requirements.

NinJo is programmed entirely in JAVA. As a result, the workstation system can be installed on different operating systems (e.g. Unix, Linux and Microsoft Windows). This avoids the necessity of porting the source code onto a specific operating system.

In principle, NinJo is able to run on any computer, be it a laptop or a supercomputer. However, adequate hardware for the expected volume of data is necessary. Both the client and server platforms need to have sufficient main memory and processor speed. In addition, a sufficiently fast network connection is required.

NinJo relies on some external systems, e.g. for file handling, decoding of meteorological reports and bulletins, document management and scheduling.

On the NinJo Server, different import and data servers are responsible for the importing of the data and making it accessible to the Clients. Furthermore, the NinJo server comprises 

- the Event Service for the automatic warning (notifications to the Clients),
- Export Services, e.g. for warnings or products,
- Infrastructure Services, and
- the Production Services, e.g. for the NinJo Batch System, Application Servers or Web Services.

On the client side, there is the NinJo Workstation for

- Visualisation,
- Monitoring,
- Production of warnings,
- Interactive editing and
- Configuration of NinJo Batch products.

**Data Flow**

NinJo receives data from different sources and in various formats.

Meteorological data is imported into the system via configurable import modules. Before the data is ingested into NinJo via the import services, it may need to be decoded using external systems. Best suitable are the following systems:

- GloBUS to decode the whole bunch of meteorological alphanumerical and binary weather formats and
- PyTROLL to preprocess data from geostationary and polar orbiting satellites. 

After the import, the data is stored on the data servers and also made available for server applications, such as the Event Service for the automatic warning procedure AutoMON. The NinJo Server then provides the data to the NinJo Client applications.

Visualisations are only generated when the query is posed. Thus, they are always up-to-date. 

![Data flow](DataFlow.png)

**Hardware platform**

The used hardware platform should be Intel or AMD based and have a x86 architecture. Both 32-bit and 64-bit systems are supported.

**Client/server architecture**

The NinJo software is client/server based. On the server side, the NinJo Servers and Services can be distributed on several machines comparable to a grid computing cluster. For higher data throughput, it is recommended to use a two server setup and distribute the various Servers and Services on these two machines.

**Supported operating systems**

Both server and client software run on Windows and Linux systems. Commonly, the NinJo Server runs on Linux, the NinJo Client on Windows. It is also possible to use Linux for the NinJo Clients or a Windows server for the NinJo Server.

**Integrated data formats**

As NinJo is used internationally, a large number of different data types is  already integrated into NinJo. NinJo has a very modular and scalable design. Therefore, new data formats for visualisation in the existing layers can easily be integrated upon request.

Amongst others, the following data formats are already integrated:

**Observation data**

- SYNOP: SYNOP FM12 (surface synoptic observations from stationary land stations), SYNOP SHIP FM13 (global surface synoptic observations from sea stations), SYNOP MOBIL FM14 (global surface synoptic observations from mobile land stations), MREP (regional reports about hazardous weather phenomena), SWN (DWD storm warn network: asynoptic strong wind reports), SWNCH (MeteoSwiss storm warn messages), GEWE (DWD: hazardous weather repors from non-professional observers), WEHI (DWD: weather repors from non-professional observers), MN2000 (universal data set from AMDA, the Meteorological Network 2000), VNORM/SYNOP
- METAR: METAR FM15, SPECI FM16
- BUOY: BUOY FM18
- PILOT: PILOT FM32 (upper air wind reports from stationary land stations), PILOT SHIP FM33 (upper air wind reports from sea stations), PILOT MOBIL FM34 (upper air wind reports from mobile land stations)
- TEMP: TEMP FM35 (upper air soundings from stationary land stations), TEMP SHIP FM36 (upper air soundings from sea stations), TEMP DROP FM37 (upper air soundings from drop sonde measurements), TEMP MOBIL FM38 (upper air soundings from mobile land stations)
- Aircraft reports: CODAR/AIREP FM41, AMDAR FM42
- TRACKOB: TRACKOB FM62
- TESAC: BATHY FM63 (temperature, salinity and current report from a sea station), TESAC FM 64 (temperature, salinity and current report from a sea station)
- ocean profiles from [Argo floats](http://www.argo.net/)
- SATEM: SATEM FM86 (upper air soundings from satellite measurements)
- Other FM20, FM22, FM39-40, FM71, FM72, FM75, FM76,
- Aviation reports: SIGMET, AIRMET, GAMET, TAF, GAFOR, 
- Wind profile data from wind profiler, SODAR and LIDAR measurements
- MeteoSwiss ANETZ (automatic observation network) and ENETZ (additional observation network)
- DWD NSD (precipation and snow reports from non-professional observers)
- DWD SWIS (road conditions for Germany)
- DWD WISPO (winter sport conditions)
- RAD_DWD (DWD radioactivity reports)
- Bulletins: mch_db (Meteoswiss decoded bulletins)

All GTS WMO alphanumerical code forms and BUFR code forms (BUFR3 and BUFR4) are decoded for NinJo by GloBUS4NinJo.

**Point forecast data**

- native formats, O_* (DWD point forecast), Hirlam (KNMI point forecast)

Other formats are easily integrated (e.g. FIMOS (DWD point forecast).

**Lightning data**

- Vaisala, SFERICS, SFUK45, SFUK39, NCM, CLDN, ILRN, Météorage, DMILDN, SAFIR, UALF

**Storm cell data**

- CARDS, KONRAD (SCIT), TRT, SAC, RDT, TITAN, CellMOS, Mesocyclones

**Satellite data**

- GeoTIFF, PNG, JPG, HDF5, …

**Satellite wind data**

- HRW, IASI, ASII, scatterometer winds

**Radar data**

- DWD radar format, DMI radar format, MeteoSwiss radar format, TITAN, MIRAN, TRT, CARDS as OPERA BUFR, NetCDF, HDF5, Beijing 08 compatible

**NWP model data**

- GRIB: GRIB1, GRIB2
- netCDF
- regular grids

**Trajectory data**

- DWD BUFR format for trajectories from GME, LME and LMK)
- KNMI format

**Station catalogues**

- WMO, ICAO, local, native via database, generic tool available to create defined catalogue

**Bulletins**

- decoded and in original form
    
**Available map projections**

- All projections defined by the Proj4 library
- Lon/Lat projection
- Geograph Grib projection
- Gnomonic projection
- Grib projection
- Hammer projection
- Kepler projection
- Lambert Cylindrical projection
- Lambert Polar projection
- Local Lambert Conformal projection
- Mercator projection
- Polar Stereographic Grib projection
- Polar Steographic projection
- Rotated Geograph Grib projection
- Stereographic projection
- Stereographic South projection
- UTM projection

NinJo contains a set of pre-configured maps. You can easily extend this set to suit your own needs using the MapCreator tool, which is also part of NinJo.
