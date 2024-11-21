# Thermistor Library

## Description
This library provides tools to measure temperature using a thermistor and an Arduino board.

## Author
- Name: DREYER Victor
- Email: victor.dreyer02@gmail.com
- Date: 2024-11-18

## Usage
- Include the library in your project.
- Initialize a Thermistor object with your specific parameters (Rref, R0, Beta, etc.).
- Use the `getTemperature` function to measure the temperature in Kelvin, Celsius, or Fahrenheit.

## Example
Variable Definitions
Here are the key variables used in the code:

Rref: The reference resistance of the thermistor at the reference temperature (
T
0
T 
0
​
 ), typically given in Ohms.

Example: Rref = 1000.0 for a thermistor with 
R
R = 
1
k
Ω
1kΩ at 
2
5
∘
C
25 
∘
 C.
R0: The fixed resistor value in the voltage divider circuit, also in Ohms.

Example: R0 = 1200.0.
Beta: The thermistor's Beta coefficient, a characteristic of the thermistor material, given in Kelvin.

Example: Beta = 3275.0.
T0: The reference temperature in Kelvin, typically 
298.15
K
298.15K (
2
5
∘
C
25 
∘
 C).

Example: T0 = 298.15.
Vcc: The supply voltage for the circuit, often 
5
V
5V.

Example: Vcc = 5.0.
adcResolution: The resolution of the ADC (Analog-to-Digital Converter), usually 10 bits for Arduino UNO.

Example: adcResolution = 10.
adcValue: The digital value read from the ADC, ranging from 
0
0 to 
2
adcResolution
−
1
2 
adcResolution
 −1.

Example: adcValue = analogRead(A0).

## Schematic
- A thermistor is connected in series with a fixed resistor.
- The middle point is connected to an ADC pin.
![{ED0BA5C7-7322-4BA2-B599-808593129A7D}](https://github.com/user-attachments/assets/e39b7bf5-85a0-4b27-8884-6fb1f122696a)
