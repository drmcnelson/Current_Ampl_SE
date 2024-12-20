# Current_Ampl_SE

This a two stage current amplifier with gains from 10<sup>2</sup>V/A to 10<sup>7</sup>, with a parts cost of about $40.
The design is based on the OPA656 which boasts input current noise 5fA/&#8730;Hz and input voltage noise 6nV/&#8730;Hz.
The newer OPA814 is a drop in replacement with input current noise 11fA/&#8730;Hz and input voltage noise 5.3nV/&#8730;Hz.
This repo provides gerbers, schematic and bill of materials.   For power, you need +/-5V.   See the power supply posted [here](https://github.com/drmcnelson/Dual-pos-neg-5V-Supply-from-USB-power).

In my work, measuring nano currents in organic electronics, this works better for me than the commercial items at about 1/100 of the cost.
For one thing, because it is a small board (65mmx50mm), it can be positioned close to the sample with a short run of wire, an important feature for micro and smaller current measurements.

The input pin is a virtual ground, as is usual with current amplifiers.
So, you insert this between the return from your sample and actual ground.
Gains are set by jumpers.  The first stage is in powers of 10<sup>2</sup>V/A up to 10<sup>6</sup>V/A, the second stage is x1 or x10.
The output goes to your analog input.

<img src="https://github.com/user-attachments/assets/5c1e581a-fe25-4cd3-a111-0efa3e4a9bc4" style="width:80%"/>

<br />

### Output can be bipolar
Because this board can produce positive or negative outputs, depending on your experiment,
it is a good idea to make sure that your analog input can acccept bipolar signals or is protected, for example by adding some didoes.

  <img src="https://github.com/user-attachments/assets/4868ce79-efb6-4609-96c3-aa9d4ecf298f" alt="protectiondiodes" style="width:40%"/><br />
 
