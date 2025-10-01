# Bill of Materials (BOM)

## Complete Component List

| SL | Component Name | Per Unit Cost (BDT) | Quantity | Total Cost (BDT) |
|----|----------------|---------------------|----------|------------------|
| 01 | LED (Red/Green/Yellow) | 1 | 50 | 50 |
| 02 | 2-pin Push Button | 3 | 10 | 30 |
| 03 | Resistors (1kΩ, 100Ω) | 0.20 | 200 | 40 |
| 04 | Breadboard | 85 | 15 | 1,275 |
| 05 | Jumper Wire (M-M) | 60 | 12 packs | 720 |
| 06 | F-Header | 10 | 3 | 30 |
| 07 | 7404 (NOT gate) | 1 | 15 | 15 |
| 08 | 7432 (2-input OR gate) | 5 | 15 | 75 |
| 09 | 7411 (3-input AND gate) | 10 | 16 | 160 |
| 10 | 7408 (2-input AND gate) | 10 | 15 | 150 |
| 11 | 7474 (D flip-flop) | 18 | 28 | 504 |
| 12 | 7486 (XOR gate) | 2 | 18 | 36 |
| 13 | 4072 (4-input OR gate) | 2 | 25 | 50 |
| 14 | Accessories (wires, connectors) | - | - | 300 |

**Total Project Cost: 3,435 BDT** (≈ $31 USD)

---

## IC Specifications

### Logic Gates

| IC Number | Type | Gates per IC | Supply Voltage | Propagation Delay |
|-----------|------|--------------|----------------|-------------------|
| 7404 | Hex Inverter | 6 | 5V | 12 ns |
| 7408 | Quad 2-input AND | 4 | 5V | 15 ns |
| 7411 | Triple 3-input AND | 3 | 5V | 15 ns |
| 7432 | Quad 2-input OR | 4 | 5V | 15 ns |
| 7486 | Quad 2-input XOR | 4 | 5V | 30 ns |
| 4072 | Dual 4-input OR | 2 | 5V | 60 ns |

### Sequential Logic

| IC Number | Type | Flip-flops per IC | Supply Voltage |
|-----------|------|-------------------|----------------|
| 7474 | Dual D Flip-flop | 2 | 5V |

---

## LED Specifications

- **Operating Voltage**: 2.0 - 2.2V (Red), 3.0 - 3.2V (Green)
- **Forward Current**: 20 mA
- **Colors Required**: Red (20), Green (20), Yellow (10)

---

## Resistor Values

- **1kΩ** - Used for LED current limiting
- **100Ω** - Used for pull-up/pull-down configurations
- **Tolerance**: ±5%
- **Power Rating**: 1/4W

---

## Pushbutton Specifications

- **Type**: Momentary, normally open
- **Contact Rating**: 50mA at 12V DC
- **Debounce**: Hardware debouncing not implemented
- **Mounting**: Through-hole

---

## Power Requirements

- **Supply Voltage**: 5V DC regulated
- **Current Consumption**: ≈ 500 mA (maximum, all LEDs lit)
- **Recommended Power Supply**: 5V 1A adapter

---

## Optional Components for PCB Version

| Component | Quantity | Purpose |
|-----------|----------|---------|
| PCB Board (custom) | 1 | Replace breadboards |
| DC Power Jack | 1 | Power input |
| Power switch | 1 | On/off control |
| Voltage regulator (7805) | 1 | Voltage regulation |
| Capacitors (100µF, 0.1µF) | 10 | Power decoupling |

---

## Sourcing Notes

- ICs: Standard 74-series available from most electronics distributors
- LEDs: Common 5mm through-hole type
- Pushbuttons: Standard tactile switches
- Breadboards: 830 tie-points recommended
- Prices based on Bangladesh market (2023)

---

## Alternative Components

### Budget Options
- Replace breadboards with perfboard for permanent build
- Use 74LS series ICs (lower power consumption)
- Reduce number of breadboards with careful layout

### Premium Options
- Use 74HC series for faster operation
- Add LED drivers for brighter display
- Use illuminated pushbuttons

---

**Note**: Prices and availability may vary by region and supplier. Check local vendors for current pricing.
