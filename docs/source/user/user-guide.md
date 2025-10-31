PDS4 Instrument Type (CTLI) Data Dictionary User's Guide

October 27, 2025

L.F. Huber

# Introduction

## Purpose of this User's Guide

This guide describes the organization and contents of the Instrument Type (CTLI) Data Dictionary, one of several Data Dictionaries maintained by the Planetary Data System (PDS). This dictionary is used when creating labels for instrument context products.

## Audience

This guide is intended primarily for use by PDS personnel (or their international equivalents). Context products should be both created and curated by the PDS.

## Applicable Documents

**The Planetary Data System Standards Reference**, <https://pds.nasa.gov/datastandards/documents/sr/current/>, the complete reference for the PDS4 Information Model

**The PDS4 Data Dictionary**, <https://pds.nasa.gov/datastandards/documents/dd/current/>, the PDS4 core (or "common") dictionary in an easily searchable HTML format

**The PDS4 Information Model Specification**, <https://pds.nasa.gov/datastandards/documents/im/current/>, the same information as in the PDS4 core dictionary, in a formal specification for use by programmers and data engineers

# Overview of the Instrument Type Data Dictionary

The Instrument Type Data Dictionary provides a way to classify instrument types. It also allows for similar types to be connected to each other to aid in search. This dictionary is only for use in instrument context products and so should only be used by PDS personnel when creating context products to associate with archive bundles.

The Instrument Type Data Dictionary is controlled by a Steward Team, the current lead of this team is Lyle Huber at the PDS Atmospheres Node (<lhuber@nmsu.edu>).

# How to Include the Instrument Type Data Dictionary in a PDS4 Label

Here is an example of how this dictionary might be used in an instrument context product:

&lt;Instrument&gt;

&lt;name&gt;Radio Science Subsystem&lt;/name&gt;

&lt;Type_List_Area&gt;

&lt;ctli:Type_List&gt;

&lt;ctli:type&gt;Radio Science&lt;/ctli:type&gt;

&lt;/ctli:Type_List&gt;

&lt;/Type_List_Area&gt;

&lt;naif_instrument_id&gt;not applicable&lt;/naif_instrument_id&gt;

&lt;serial_number&gt;not applicable&lt;/serial_number&gt;

&lt;description&gt;

The telecommunications system uses an X-band transponder on the spacecraft and

transmitters and receivers at stations of the NASA Deep Space Network on Earth.

Range and Doppler measurements made during communcations sessions can be used to

determine the spacecraft trajectory; from the trajectory, Mercury's gravity field

can be inferred. Measurements of occultation times can be used to obtain the

planet's radius at the occultation points, refining the planet's shape model.

&lt;/description&gt;

&lt;/Instrument&gt;

# Values and their Definitions

- Accelerometer: An accelerometer measures acceleration -- rate of change of velocity -- in its own rest frame.
- Altimeter: An altimeter measures distance above a surface. (Close match with Lidar.)
- Atmospheric Structure Instrument: An atmospheric structure instrument measures one or more structural properties of an atmosphere. These properties may include -- but are not limited to -- pressure, temperature, density, wind speed, and wind direction. (Close match with Meteorology. Close match with Weather Station.)
- Camera: A camera is an optical instrument that captures a still image or a sequence of images on physical media. (Exact match with Imager.)
- Charged Particle Detector: A charged particle detector detects and/or counts charged particles, and provides information about particle properties and distributions.
- Chemical Analyzer: A chemical analyzer uses sensors to detect the products of reactions when samples are mixed with known reagents.
- Dust Analyzer: A dust analyzer measures the size and/or energy distribution of dust particles.
- Electric Field Instrument: An electric field instrument measures the direction and/or strength of an electric field.
- Gamma Ray Detector: A gamma ray detector is an instrument that detects gamma rays.
- Gas Analyzer: A gas analyzer measures the concentration of one or more species in a mixture of neutral gases.
- Gravimeter: A gravimeter measures gravitational acceleration.
- Imager: An imager detects and converts information into a digital image. (Exact match with Camera).
- Imaging Spectrometer: An imaging spectrometer acquires a spectrally-resolved image of an object or scene. Two axes of the image correspond to orthogonal spatial dimensions and the third corresponds to wavelength.
- Interferometer: An interferometer superposes waves such that constructive and destructive interference results in patterns that can be interpreted as very small displacements at the signal source.
- Langmuir Probe: A Langmuir probe consists of one or more electrodes used to determine in-situ plasma properties such as density and temperature from the measured potentials and currents.
- Lidar: A lidar measures distance to a target by illuminating it with a pulsed laser and measuring the time delay of the reflected signal. (Close match with Altimeter.)
- Magnetometer: A magnetometer measures the direction and/or strength of a magnetic field.
- Mass Spectrometer: A mass spectrometer sorts and counts atoms, ions, and/or molecules based on their masses.
- Mechanical Properties Instrument: A mechanical properties instrument measures the reaction of a sample to an applied load, quantifying properties such as strength, stiffness, ductility, hardness, fracture toughness, and/or friability.
- Meteorology: A meteorology instrument measures in situ meteorological conditions. These may include -- but are not limited to -- pressure, temperature, wind speed, and wind direction. (Exact match with Weather Station and Close match with Atmospheric Structure Instrument.)
- Microphone: A microphone converts sound waves into electrical signals.
- Microscope: A microscope magnifies objects that are too small to be seen with the naked eye.
- Mutual Impedance Probe: A mutual impedance probe measures in situ bulk plasma properties at radio frequencies.
- Nephelometer: A nephelometer measures the concentration of suspended (cloud) particulates.
- Neutral Particle Detector: A neutral particle detector detects and/or counts neutral particles, and provides information about particle properties and distributions.
- Neutron Detector: A neutron detector detects and/or counts neutrons.
- Photometer: A photometer is an instrument that measures the brightness of light without spatial or spectral resolution.
- Plasma Wave Receiver: A plasma wave receiver detects waves in the local plasma medium using electric or magnetic antennas.
- Polarimeter: A polarimeter measures the polarization of an electromagnetic wave.
- Precision Scale: A precision scale is a device used to measure the mass of a sample.
- Radar: A radar transmits an electromagnetic wave, then measures amplitude, time delay, frequency shift, phase shift, and/or polarization of the echo from a distant target.
- Radio Receiver: A radio receiver detects the information in propagating electromagnetic waves collected by an antenna.
- Radio Science: Radio science is the use of active and/or passive electromagnetic waves to probe the environment.
- Radiometer: A radiometer measures radiant flux (power) of electromagnetic radiation.
- Relaxation Sounder: A relaxation sounder determines the properties of a plasma by actively probing at radio frequencies at and near the plasma frequency.
- Retroreflector Array: A retroreflector array consists of multiple objects that reflect light back towards its source.
- Seismometer: A seismometer measures ground motions such as might be caused by earthquakes, volcanic eruptions, or explosions.
- Spacecraft Sensor: A spacecraft sensor captures information on the status or physical condition of a spacecraft or its components. These may include, but are not limited to, temperatures, mechanical friction, currents, voltages, etc.
- Spectrometer: A spectrometer measures an energy spectrum.
- Spectrum Analyzer: A spectrum analyzer measures the properties of photons, charged particles, or electrical signals as a function of frequency or energy.
- Sub-Surface Tool: A sub-surface tool probes the upper few meters of a surface to infer its properties. Examples include (but are not limited to) drills and penetrators.
- Surface Tool: A surface tool physically probes a surface to infer its properties. Examples include (but are not limited to) brush and deployment systems.
- Temperature Sensor: A temperature sensor measures temperature.
- Weather Station: A weather station is a suite of instruments that measures in situ meteorological conditions. These may include -- but are not limited to -- pressure, temperature, wind speed and wind direction. (Exact match with Meteorology and Close match with Atmospheric Structure Instrument.)
- Wind Tunnel: A wind tunnel is used to study the effects of air moving past solid objects.

