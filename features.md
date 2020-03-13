
The basic visualisation concept of NinJo is the presentation of data in separate layers. Users can add as many layers to a NinJo scene as they want (restricted only by memory amount of hardware). All layers show time-synchronised data for the same map area in the so-called NinJo scenes.

The layers are independent and can be added and removed from the scenes separately. If they are added to a scene, they can be set visible or invisible. Furthermore, their transparency is continuously adjustable.  

Layers can be arranged in any order the users want enabling them to arrange all data types according to their specific needs.

# Surface Layer

The Surface Layer displays observed and point-forecast data. Formats such as SYNOP, METAR, MREP and SPECI are supported.

A versatile configuration of the display modes (symbols, plot models, values, isolines, isoareas) is possible. A very large amount of preconfigured data display modes is available, new ones can easily be created. Preconfigured plotting modes for observational data are, for example, the WMO station plot, the plot for significant weather, and specified elements (e. g. temperature in 2 m height, total cloud cover or wind direction). In principle, all combinations of all available elements are possible.

The reports can also be displayed or listed in the original text format. Furthermore, the Bulletin Viewer visualises bulletins in the NinJo Client and allows the seraching and filtering of bulletins according to their header information as well as selecting, viewing and copying of the bulletin content.

The Surface Layer also serves to create observation-based meteograms for any available station.

# NWP-Model Layer

The NWP-Model Layer displays data of all numerical weather prediction (NWP) models, such as GME, GFS or ECMWF. 

Furthermore, calculated elements, e.g., precipitation sums or differences, can be displayed directly.

The user can switch between models, model runs and forecast times. Models with the same forecast time or different model runs of the same forecast time can easily be compared with each other.

The visualisation of the model data is very flexible and can be configured according to your specific requirements. NinJo supports isolines, isoareas, numbers or symbols and windbarbs. All colors, line types, line attributes, etc. can be configured.

# Satellite Data Layer

The Satellite Data Layer visualizes all available channels of geostationary satellites, such as GOES, GMS and Meteosat, and polar-orbiting satellits, such as the NOAA and MetOp satellites. NinJo produces a "world mosaic" satellite image from the geostationary satellites.

Furthermore, you can create satellite composites using three different channels, , for example for a better visualization of high or low clouds. In order to allow easy access to such composites, you can adapt the myGUI panel of the Satellite Data Layer. The myGUI panel summarizes the most important configuration settings for each layer so that you can quickly change these settings without having to change the active layer.

You can also display the products of the Satellite Nowcasting Facility (Nowcasting SAF). 

The Satellite Data Layer offers a flexible color configuration for all values as well as two different modes of contrast enhancement. The substraction of channels is also possible. 

# Radar Layer

The Radar Layer enables the user to select between the different radar products available . It is also possible to visualize the product of one selected station. Furthermore, you can define a cross section through an area of precipition 

# Aviation Layer

The aviation layer meets the special needs of aviation forecasting. Supported are GAFOR, GAMET, AIRMETSIGMET, METAR and TAF reports.

The user can define a flight path (also with stopovers) and get all reports for it. 

The reports can be copied to the clipboard, to use it in another program, or be printed directly. 

# Sounding Layer

In the Sounding Data Layer, radiosonde measurements and wind profile data as well as derived parameters are visualized as plot elements or plot element groups. In addition, the layer offers easy access to the Sounding Application.

The Sounding Application is used to visualize and analyze data of atmospheric vertical soundings. The sounding data originates from radiosonde ascents, aerological drop sondes, wind profilers or satellites.

Oceanographic soundings from ship measurements and measurements by drifting buoys or profiling floats can be visualized in the Ocean Profile Application. A large number of measured and derived parameters, for example different thunder-storm indices, are available from the default configuration of the layer-specific menu. 

# SatSounding Layer

The SatSounding Layer displays point data derived from satellite data ("Infrared Atmospheric Sounding Interferometer" (IASI). Comparable to the radiosonde ascents you can compare and analyse its data using the sounding application.

# SatWind Layer

The SatWind Layer is a point data layer and can display computed wind data from satellite images. The layer displays high resolution wind data as well as scatterometer winds.

The software package developed by SAFNWC (Nowcasting Satellite Application Facilities) allows calculating up to twelve different main products including wind vectors based on successive sequences of the high resolution broadband channel in the visible range (HRV channel, 600-900nm). Data is available throughout the day for Europe, North Africa and the adjoining seas. 

# SatFeature Layer

The Network of Satellite Aplication Facilities (NWC SAF) makes a product available, which bears on the automatic interpretation of the satellite image (Automatic Satellite Image Interpretation, ASII). The satellite images are analysed with the aid of conceptual models. They constitute a synthesis of physical processes and the typical outward forms (features) that the processes in satellite images or other synoptic data bring about. The analysed data comes from SERVIRI instruments (Spinning Enhanced Visible and Infrared Imager) on board of the MSG-satellites (Meteosat Second Generation).

The basis of the image interpretation are so-called pattern recognition methods, which are used to investigate the form and position of typical cloud appearances in the satellite image. The following forms of appearance were detected:

- Frontal zones
- S-Shaped lines
- Circular cells
- Narrow cloud bands
- Black stripes in water vapour images
- Spiral-shaped cloud structures

# SCIT (storm cell identification and tracking) layer

The SCIT layer displays storm cell data. Storm cells can be visualised as one-size cirles (all cells have the same size, e.g. used at the DWD) or in real size (used at the South African Weather Service).

Cells can be tracked, the movement and velocity can be displayed. All current cells can be listed in a table, the selected cell is displayed seperately at the bottom. Also, if available in the data, secondary cells and cell forecasts can be displayed. 

# Lightning layer

The lightning layer displays the reported lightnings of a selected network for the configured time period.

Lightnings can be colored by age or type, polarity, intensity, stroke count or quality. Positive and negative strokes as well as cloud-to-ground strokes can be displayed seperately. 

# Road Weather Layer

The Road Weather Layer displays observational data of the GMAs and forecasts of AutoSWIS and describes the status of roads and highways.

Road meteorological data is displayed in the form of plot elements and plot element groups in a similar manner as in the Surface Data Layer.

# MOS Layer

The MOS Data Layer shows the results of the Model Output Statistics Method. Its layout is comparable to that of the Surface Data Layer. They just differ in the selection of plot elements and plot element groups.

# Ocean Profile Layer

The Ocean Profile Layer shows the data of the Argo buoys. Argo is an international observation system with buoys that probe salinity, ocean temperature and the concentration of oxygen dissolved in the water down to a depth of two kilometres.

Electrical conductivity, potential density, sound speed and the sound speed gradient are computed by the data obtained.

Data can be visualised and compared in diagrams or in tables. 

# AutoMON Application

NinJo comprises the AutoMON application, which handles warnings. All warning criteria (rules) can be fully configured. The AutoMON sever reads the appropriate ingested data and checks it against the existing rules. Rules can be configured per user/client or on a side or system wide level. Users can define their own rules and activate them according to their needs. Whenever data matches a rule, the client is informed by the AutoMON server. Signal lamps show the status of events. An own client side AutoMON application can be started to configure the AutoMON rules as well as to  confirm warnings.

Currently, observational data, point forecast data, lightning data and radar data can be monitored. Other data types will be integrated in the future. 

# Trajectory Layer

The Trajectory Layer visualises forward and backward trajectories of the GME, LME and LMK model for pre-defined locations to reconstruct the movement of air parcels. Trajectories can be shown for different height levels and in different colour saturations. 

# Webcam Layer

The Webcam Layer displays webcam images in the NinJo Client to give the forecaster an idea of the current weather situation. A webcam symbol indicates the locations of webcams. The user can add own webcams to the NinJo webcam list. All webcams on the internet can be added. 

# Geographical layers

NinJo visualizes meteorologic and oceanographic data on maps. The geographical background and references are provided by five different layers:

- Raster layer
- Vector layer
- Gridlayer
- ??
- ??
 

There are three geographical layers available: one for raster data, one for vector data and one for displaying the grid of parallels and meridians.

For raster data, different data sets are available (height/elevation, landuse, satellite images, ...). Vector data contains information about coastlines, boundaries, cities, roads, rivers, airports, etc. Which data shall be displayed and with which colors, lines and line attributes, can be configured by the user.

NinJo supports an intelligent level-of-detail display, that means, the more the user zooms in, the more data he sees. The resolution of the images is adapted automatically. 

Furthermore, NinJo contains the following components:

- Product Workbench to produce synoptic charts, e.g., the Significant Weather Chart SWC, as well as
- NinJo Batch to generate products automatically.

# Animations

Where necessary, map displays (e.g. radar or satellite images) can be played back as an animation over certain time domains. This allows the evolution of both past events and predictions to be visualised.

The animation feature is available for all layers and all zoom levels. Each of the scenes (max. one main and three secondary scenes) can be animated individually. The time range, interval, and animation speed is set by the user (see Figure 7).

Auto updating of all data is also supported while running an animation. NinJo currently checks once a minute for new data and updates the necessary animation frames. 

# NinJo Applications

The superiority of NinJo is evident especially in the modular principle of construction comprising different layers and applications that are available to the user. In one and the same window, it is possible to open several scenes with different areas of work. All visualisations are not generated until the instant of querying and, as a result, are always right up-to-date. Data comes directly from the servers.

Besides the main window, further secondary windows can be opened. The entire set of windows and scenes comprises the work session, which is stored as a configuration and called up with the same layout the next time the program is started.

No matter whether your work involves station data, satellite images, weather maps, warning messages, radio soundings, meteograms etc.: NinJo has not only extensive forms of representation but also, in its Enterprise edition, offers experienced software developers the option of producing their own layers and applications.

# Meteograms, Cross-Sections, Soundings

NinJo supports the creation of meteograms and soundings for specific station data or model data. Different models (meteograms) or stations (soundings) can be compared with each other. Also, the creation of vertical cross-sections is possible.

# Graphical Editor

The graphical editor allows the user to create weather maps. Standard functions include, for example, drawing-in or alteration of fronts, jet streams, severe areas as well as marking of storm cells and the like. It also allows the meteorologist's experience and knowledge to be directly brought to bear on the weather map. On screen drawing is supported by connecting an interactive pen display.

# Configuration

The NinJo main window with one so-called main and up to three separate secondary scenes is just the framework around various areas. Each scene can comprise a variable number of layers which are arranged in the layer bar. All user specific configuration parameters such as selection of layers and scenes, time slots, arrangement of windows etc. are stored on the server. At next login the user will start with the same configuration even if he resumes the work at another client computer.

Most of the system configuration can be done interactively. The configuration of XML files can be adjusted by the customers themselves, if necessary. Depending on the configuration, NinJo may be started either with one or more display screens, or with one or more windows and layers. Its design resembles the building-block principle.

NinJo is open for further layers and applications. Customer-specific extensions or alterations can be implemented according to requirements.
