# SCCM Simulink Test Environment

This repository contains a Simulink-based Hardware-in-the-Loop (HIL) model for validating the Steering Column Control Module (SCCM).

 Components
- `SCCM_PlantModel.slx`: Simulates physical switches, paddles, steering rotation.
- `SCCM_SignalRouting.slx`: Routes and transforms signals for HIL compatibility.
- `SCCM_Testbench.slx`: Top-level test model including logging and stimuli.
- `SCCM_DataDictionary.sldd`: Contains signal metadata and calibration parameters.

 Test Environment
- Toolchain: MATLAB Simulink + dSPACE (ControlDesk/AutomationDesk)
- Protocols: CAN, LIN, Analog I/O, Digital I/O
- Integration: Designed to work with dSPACE HIL and VT System

HIL-testbench-setup
SCCM_Simulink_TestSetup/
├── README.md
├── Simulink_Model/
│   ├── SCCM_Testbench.slx
│   ├── SCCM_PlantModel.slx
│   ├── SCCM_SignalRouting.slx
│   └── SCCM_DataDictionary.sldd
├── Docs/
│   ├── TestSetup_Architecture.pdf
│   ├── SignalDescription.xlsx
│   └── ModelDescription.md
└── Scripts/
    └── Init_Simulation.m


