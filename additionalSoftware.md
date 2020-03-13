# Additional Software

## GloBUS - Decoding meteorological messages
GloBUS is a modern coding/decoding system that is adopted for central decoding of weather reports of different codes (mainly point data formats such as SYNOP, TEMP, PILOT and METAR). Decoded input reports can be transferred to different output formats, such as BUFR Edition 3 or BUFR Edition 4. For the creation of BUFR output reports, the new BURF templates proposed by WMO are supported. GloBUS4NinJo creates a special CORBA object and provides it for the NinJo import systems.

Decoding of weather reports in the system GloBUS is performed independently of the specific input and output formats. Reports of different codes are translated in a standardised way by the system and transformed into a universal and fully documented internal format. This format is then translated into the required output format to be imported into NinJo. This allows the simple extension of the system to support new input and output formats.

The system was developed completely in JAVA and can therefore be used on any platform that includes a JAVA installation. The GloBUS system can be run on expensive servers as well as on a single laptop. The system works independently from databases. All required data is stored in XML format which can be stored as text in any perceivable database. The system GloBUS is flexible, extendable and highly configurable due to the strict separation of its different components. 

## SKY - Meteorological report database

In order to meet the growing demands placed on the storage of meteorological data, the product SKY has been developed. The software can be used for the long-term storage and access of daily weather reports. In particular, SKY is designed to cope with the storage of the rapidly rising volumes of satellite and radar data.

With the use of state-of-the-art software technologies, the new report database SKY is suitable ofr handling various types and quantities of data. The system is based on a multi-layer architecture and the combination of a relational database and storage in a file system.

Prominent features of SKY are:

- Component and object-oriented multi-layer architecture
- Upgradable performance
- Compressed storage in file system and database possible
- Integration of external applications via XML-interfaces
- Flexible structuring of the data

Special emphasis was placed during the development of SKY on the performance, scalability and portability. In addition, users and administrators are supported by graphics tools.

The system is basically format neutral. That means that almost all sorts of data can be stored. SKY can be coupled together with GloBUS and also with an archive systems.

If you wish more information, please do not hesitate to contact us.
