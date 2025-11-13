<h2>Description of the sub-circuits.</h2>

**1. Voltage Quadrupler**
* A voltage quadrupler is a diode–capacitor charge-pump network that multiplies the peak value of an AC input by approximately four.
* It works by charging capacitors on alternating AC cycles and stacking their voltages in series.
* The result is a much higher DC voltage than the original AC input.
* It is commonly used when a circuit requires a high DC level, but the available AC supply is low and a transformer is not desired.
* In short: low-voltage AC → high-voltage DC.



**2. LDO (Low Dropout Regulator)**
* An LDO is a linear regulator designed to maintain a stable, low-noise DC output even when the input voltage is only slightly higher than the desired output.
* It removes ripple, noise, and variations from the quadrupler’s output.
* It provides a clean, precise DC voltage for sensitive analog stages.
* Because it’s a linear device, it has excellent noise performance compared to switching regulators.
* In short: noisy DC in → clean, regulated DC out.

**3. Common Source Amplifier**
* A common source amplifier is a fundamental MOSFET amplifier topology used for voltage gain.
* The source terminal is common (usually tied to ground), the input signal is applied to the gate, and the output is taken from the drain.
* Small-signal behaviour:
    * It provides significant voltage gain because variations in gate voltage modulate the drain current, which produces amplified voltage swings across the load resistor.
* Large-signal behaviour:
    * It describes the full transistor operation, considering nonlinearities and the transistor’s actual I–V curves (cutoff, triode, saturation).
* It determines the maximum output swing, bias point, and distortion limits.
* In short: AC signal in → amplified AC signal out.

<h2>Photos</h2>

<h3>Schematic</h3>

![alt text][schematic]

<h3>PCB Front</h3>

![alt text][layout-front]

<h3>PCB Back</h3>

![alt text][layout-back]

<h3>3D Model</h3>

![alt text][threed-model]


[schematic]: https://github.com/Ryan-Perera/PCBs/blob/main/Schematic.png
[layout-front]: https://github.com/Ryan-Perera/PCBs/blob/main/Layout-Front.png
[layout-back]: https://github.com/Ryan-Perera/PCBs/blob/main/Layout-Back.png
[threed-model]: https://github.com/Ryan-Perera/PCBs/blob/main/3D-model.png
