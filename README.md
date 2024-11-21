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
See the `examples/simpleTest` folder for a sample implementation.

## Schematic
- A thermistor is connected in series with a fixed resistor.
- The middle point is connected to an ADC pin.
![{ED0BA5C7-7322-4BA2-B599-808593129A7D}](https://github.com/user-attachments/assets/e39b7bf5-85a0-4b27-8884-6fb1f122696a)
