# 📦 Bill of Materials (BOM)
## Hash Vault Elite Edition by MeridianAlgo

## Power Supply Components

| Reference | Part Number | Description | Quantity | Notes |
|-----------|-------------|-------------|----------|-------|
| U1 | TPS53647 | Synchronous Buck Controller | 1 | 0.9V ASIC core rail, >95% efficiency |
| U2 | TPS54331 | 3.3V Buck Converter | 1 | Logic and peripherals |
| Q1-Q4 | CSD95481RWJ | Dual N-Channel MOSFET | 2 | Low RDS(on) for efficiency |
| L1 | SRP1265A-1R0M | 1µH Power Inductor | 1 | High current, low DCR |
| L2 | SRP7028A-2R2M | 2.2µH Power Inductor | 1 | 3.3V rail |
| C1-C10 | GRM32ER71E226KE15L | 22µF Ceramic Cap | 10 | X7R, 25V, low ESR |
| C11-C20 | GRM188R71C104KA01D | 0.1µF Ceramic Cap | 10 | X7R, 16V decoupling |
| C21-C22 | EEE-FK1E101P | 100µF Electrolytic | 2 | Low ESR bulk caps |
| R1-R4 | RC0603FR-071KL | 1kΩ Resistor | 4 | 1% tolerance |
| R5-R6 | RC0603FR-0710KL | 10kΩ Resistor | 2 | Feedback dividers |

## ASIC & Mining Components

| Reference | Part Number | Description | Quantity | Notes |
|-----------|-------------|-------------|----------|-------|
| U3-U8 | BM1397 | Bitcoin Mining ASIC | 6 | 400 GH/s each = 2.4 TH/s total |
| Y1 | ABM8G-25.000MHZ | 25MHz Crystal | 1 | ±10ppm, low jitter |
| C23-C82 | GRM188R71C104KA01D | 0.1µF Ceramic Cap | 60 | ASIC decoupling (10 per chip) |
| C83-C106 | GRM32ER71E226KE15L | 22µF Ceramic Cap | 24 | ASIC power filtering (4 per chip) |
| R7-R30 | RC0603FR-0733RL | 33Ω Resistor | 24 | Series termination |

## Microcontroller & Communication

| Reference | Part Number | Description | Quantity | Notes |
|-----------|-------------|-------------|----------|-------|
| U9 | ESP32-S3-WROOM-1-N16R8 | WiFi MCU Module | 1 | Dual-core, 16MB Flash, 8MB PSRAM |
| U10 | W5500 | Ethernet Controller | 1 | Optional, for low-latency mining |
| U11 | CP2102N | USB-to-UART Bridge | 1 | Programming interface |
| U12 | SSD1306 | OLED Display 128×64 | 1 | Real-time stats display |
| J1 | USB4105-GF-A | USB-C Connector | 1 | 100W PD power and programming |
| J5 | RJ45-8P8C | Ethernet Jack | 1 | Optional Ethernet connection |
| C107-C115 | GRM188R71C104KA01D | 0.1µF Ceramic Cap | 9 | MCU + Ethernet decoupling |
| R31-R36 | RC0603FR-0710KL | 10kΩ Resistor | 6 | Pull-ups |
| R37-R38 | RC0603FR-075K1L | 5.1kΩ Resistor | 2 | USB-C CC pins for PD |

## Sensors & Monitoring

| Reference | Part Number | Description | Quantity | Notes |
|-----------|-------------|-------------|----------|-------|
| U13-U18 | INA219AIDCNR | Current/Voltage Monitor | 6 | One per ASIC for individual monitoring |
| U19-U24 | TMP102AIDRLT | Temperature Sensor | 6 | One per ASIC for thermal management |
| R39-R40 | RC0603FR-074K7L | 4.7kΩ Resistor | 2 | I2C pull-ups |

## Cooling & Thermal Management

| Reference | Part Number | Description | Quantity | Notes |
|-----------|-------------|-------------|----------|-------|
| FAN1-FAN2 | NF-A4x10 FLX | 40mm PWM Fan | 2 | Noctua, ultra-quiet, dual-fan system |
| Q5-Q6 | 2N7002 | N-Channel MOSFET | 2 | Fan PWM control |
| R41-R42 | RC0603FR-071KL | 1kΩ Resistor | 2 | Gate resistors |
| HS1 | Custom | Large Heatsink 150×120mm | 1 | Aluminum with optimized fins |
| TIM1 | Thermal Grizzly Kryonaut | Thermal Paste | 1 | Premium TIM, >8 W/mK |

## Connectors & Mechanical

| Reference | Part Number | Description | Quantity | Notes |
|-----------|-------------|-------------|----------|-------|
| J2 | PJ-002A | DC Barrel Jack | 1 | 12V input, 5.5mm/2.1mm |
| J3 | TSW-104-07-G-S | 4-pin Header | 1 | UART debug |
| J4 | TSW-106-07-G-S | 6-pin Header | 1 | I2C expansion |
| SW1 | TL3342F160QG | Tactile Switch | 1 | Reset button |
| D1-D6 | LTST-C191KGKT | LED Green | 6 | Per-ASIC status indicators |
| D7 | LTST-C191TBKT | LED Blue | 1 | Power indicator |
| D8 | LTST-C191KRKT | LED Red | 1 | Error indicator |
| R43-R50 | RC0603FR-07330RL | 330Ω Resistor | 8 | LED current limiting |

## PCB Specifications

| Parameter | Value |
|-----------|-------|
| Board Size | 180mm x 140mm (Elite 6-ASIC design) |
| Layers | 6 (Signal/GND/Power/Power/GND/Signal) |
| Copper Weight | 4oz (140µm) on power planes, 2oz on signal layers |
| Min Trace/Space | 6mil/6mil (0.15mm) |
| Min Drill | 0.3mm |
| Finish | ENIG (Electroless Nickel Immersion Gold) |
| Solder Mask | Green, both sides |
| Silkscreen | White, both sides |

## Assembly Notes

1. **Reflow Profile**: Standard lead-free SAC305 profile
2. **Stencil**: 4mil stainless steel, electropolished
3. **Assembly Order**: Bottom side first, then top side
4. **Critical Components**: Hand-place ASIC and ESP32 module
5. **Testing**: Program and test before heatsink installation

## Cost Estimate (Prototype Quantities)

| Category | Estimated Cost (USD) |
|----------|---------------------|
| PCB (6-layer, 4oz copper) | $80-120 |
| Power components | $50-80 |
| 6× ASIC (BM1397) | $90-150 |
| ESP32 + Ethernet + OLED | $25-40 |
| Sensors (12× INA219 + TMP102) | $30-50 |
| Heatsink + 2× Fans + TIM | $35-60 |
| Connectors + LEDs + misc | $15-25 |
| Assembly (if outsourced) | $50-80 |
| **Total per unit (prototype)** | **$375-605** |
| **Total per unit (100+ qty)** | **$200-250** |

*Costs decrease significantly at higher volumes (100+ units)*

## Sourcing Recommendations

- **PCB**: JLCPCB, PCBWay, or OSH Park
- **Components**: Digi-Key, Mouser, LCSC
- **ASIC**: Specialized suppliers or salvage from existing miners
- **Assembly**: JLCPCB SMT service or local assembly house

---

*BOM subject to change based on availability and design revisions*
