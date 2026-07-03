# Complete Technical Specifications

## Electrical Specifications

### Signal Characteristics
- **Line Rate:** 25 Gbps per lane (16 lanes = 400Gbps)
- **Signal Type:** PAM-4 (Pulse Amplitude Modulation)
- **Data Rate:** 400Gbps total / Split to 2x200Gbps
- **Operating Standard:** IBTA HDR, IEEE 802.3 400G Ethernet

### Connector Specifications

#### Input: OSFP (Octal Small Form Factor)
- 8-lane high-density connector
- 56 total pins
- MSA-compliant keying and ejector
- Hot-swappable design
- 500+ mating cycles guaranteed

#### Output: QSFP56 (2x connectors)
- 4-lane connectors per output
- 36 pins per connector
- MSA-compliant
- Hot-swappable
- 500+ mating cycles guaranteed

## Optical Specifications

### Laser & Receiver Technology
- **Laser Type:** VCSEL (Vertical-Cavity Surface-Emitting Laser)
- **Wavelength:** 850nm (Short Wavelength Multimode)
- **Fiber:** Multimode Fiber (MMF), OM4 grade
- **Core Diameter:** 50 microns
- **Cladding Diameter:** 125 microns
- **Receiver Type:** PIN photodiode
- **Sensitivity:** -11 dBm typical (excellent signal reception)

### Performance Metrics
- **Optical Path Loss:** 2.5-3.0 dB for 3m MMF @ 850nm
- **Connector Loss:** 0.5-1.0 dB per pair
- **Total Loss:** 3.5-4.0 dB (excellent margin)
- **System Margin:** >10 dB (robust design)
- **BER (Bit Error Rate):** <10^-15

## Power Specifications

### Input Power Requirements
- **Voltage:** 3.3V DC (standard data center)
- **Current:** 3.5-4.0A typical
- **Power Consumption:** 11.5-13.2W typical
- **Peak Power:** 15W (startup transient)
- **Idle Power:** 0.5-1.0W

### Heat Dissipation
- **Typical Heat Output:** 11-13 Watts
- **Thermal Resistance:** ~5°C/W
- **Case Temperature:** 40-50°C at 25°C ambient
- **Thermal Cutoff:** Auto-shutdown at >85°C

## Physical Specifications

### Cable Dimensions
- **Length:** 3.0 meters (±5 cm tolerance)
- **Diameter:** 6.5mm (including jacket)
- **Weight:** 180-200 grams
- **Bend Radius:** 30mm minimum (non-destructive)
- **Tensile Strength:** 60-80 Newton maximum

### Jacket Specifications
- **Material:** LSZH (Low Smoke Zero Halogen)
- **Rating:** Plenum-rated (US), Eca rating (EU)
- **Flexibility:** Easy hand-bending for rack routing

## Environmental Specifications

### Operating Conditions
- **Temperature:** 0°C to 70°C
- **Storage Temp:** -10°C to 80°C
- **Humidity:** 10% to 90% (non-condensing)
- **Altitude:** 0 to 3000 meters

### Safety & Compliance
- **Laser Safety:** Class 1 (safe for human exposure)
- **RoHS Compliance:** Yes (Restriction of Hazardous Substances)
- **REACH Compliance:** Yes (Chemical regulation)
- **CMIS:** 5.0 compliant

## Performance Characteristics

### Latency
- **Optical Path Latency:** ~3.5 nanoseconds per meter
- **Total Cable Latency:** ~10.5 nanoseconds for 3m
- **Active Electronics:** ~2-3 nanoseconds
- **Total End-to-End:** ~15 nanoseconds (negligible for data center)

### Reliability
- **MTBF (Mean Time Between Failures):** >50 years
- **Uptime Target:** >99.99%
- **Link Down Time:** <1 millisecond per month

## Compatibility Matrix

### Supported Systems
- ✅ NVIDIA Quantum-2 switches (400G OSFP native)
- ✅ NVIDIA Quantum-3 switches (backward compatible)
- ✅ Mellanox ConnectX-6 (200G QSFP56 native)
- ✅ Mellanox ConnectX-X6 (400G capable)
- ✅ NVIDIA DGX A100/H100 systems
- ✅ HPE Proliant GPU servers
- ✅ Dell PowerEdge GPU systems

### Firmware Requirements
- Switch firmware: Latest version supporting active optical
- Adapter firmware: Latest version recommended
- Version matching: Not strictly required

## Warranty & Support

- **Warranty Period:** 5 years from shipment
- **Manufacturing:** ISO 9001 certified facility
- **Testing:** 100% unit tested before shipment
- **Support:** Email/phone support during business hours
- **RMA Process:** Quick turnaround on defective units
