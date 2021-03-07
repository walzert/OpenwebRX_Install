######################################################
##     Soapy SDR -- the SDR abstraction library     ##
######################################################

Probe device sdrplay
[INFO] devIdx: 0
[INFO] hwVer: 1

----------------------------------------------------
-- Device identification
----------------------------------------------------
  driver=SDRplay
  hardware=B0001P0002
  sdrplay_api_api_version=3.070000
  sdrplay_api_hw_version=1

----------------------------------------------------
-- Peripheral summary
----------------------------------------------------
  Channels: 1 Rx, 0 Tx
  Timestamps: NO
  Other Settings:
     * RF Gain Select - RF Gain Select
       [key=rfgain_sel, default=1, type=string, options=(0, 1, 2, 3)]
     * IQ Correction - IQ Correction Control
       [key=iqcorr_ctrl, default=true, type=bool]
     * AGC Setpoint - AGC Setpoint (dBfs)
       [key=agc_setpoint, default=-30, type=int, range=[-60, 0]]

----------------------------------------------------
-- RX Channel 0
----------------------------------------------------
  Full-duplex: NO
  Supports AGC: YES
  Stream formats: CS16, CF32
  Native format: CS16 [full-scale=32767]
  Antennas: RX
  Corrections: DC removal
  Full gain range: [0, 42] dB
    IFGR gain range: [20, 59] dB
    RFGR gain range: [0, 3] dB
  Full freq range: [0.01, 2000] MHz
    RF freq range: [0.01, 2000] MHz
    CORR freq range:  MHz
  Sample rates: 0.0625, 0.096, 0.125, 0.192, 0.25, ..., 6, 7, 8, 9, 10 MSps
  Filter bandwidths: 0.2, 0.3, 0.6, 1.536, 5, 6, 7, 8 MHz

