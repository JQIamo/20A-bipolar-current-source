# Bias Coils Current Controller
This repo provides information regarding the Bias Coils Current Controller (here on out referred to as “the controller”) used by the Schine Group at the Joint Quantum Institute (JQI) at University of Maryland, College Park. This is an experimental apparatus designed to drive Helmholtz coil pairs to cancel external magnetic fields which would otherwise disturb the experiment. The controller provides an output current proportional to an input voltage and features an ultra-low noise feedback circuit design for precise control of the output current down to the fractional mA level. The controller has three channels to independently control the magnetic fields along the x, y, and z axes.

## 20A-bipolar-current-source
This project is based on the [`20A-bipolar-current-source`](https://github.com/JQIamo/20A-bipolar-current-source/tree/faf83a785aa46d90d6e65fa55f9879bae6bd2d8a) design of Mingshu Zhao and Alessandro Restelli. Details on the circuit can be found in their [research article in AIP Advances](https://doi.org/10.1063/5.0138145).

## Circuit files
There are several KiCad project folders within the `kicad` directory in this repo.
* `controller_board` contains the circuit board for the main controller board on which the analog PI feedback is located.
* `Controller_supply` contains the controller's on-board power supply circuit board (used for powering the controller boards)
* `H-bridge` is for the development of the MOT coil current controller (empty project as of Jun 06, 2024).
* `rear` contains the original, liquid-cooled circuit board design housing the power MOSFETs that control the coil current. (Not used in this controller)
* `SchineLab_CoilFET_Board` contains the modified, air-cooled circuit board design housing the power MOSFETs for coil current control. (Used in this controller)

