.. _top_125_14_MULTI:

###################################
STEMlab 125-14 X-Channel System
###################################

The X-Channel STEMlab 125-14 system consists of multiple Low-Noise STEMlab 125-14 devices that are modified for clock and trigger synchronisation and also comes with SATA synchronisation cables and software that supports multi-channel RF signal acquisition and generation.

X-Channel STEMlab 125-14 system consists of:

* one PRIMARY Low-Noise STEMlab 125-14 device, a standard Low-Noise STEMlab 125-14 device that provides clock and trigger signals to other SECONDARY Low-Noise STEMlab 125-14 devices.
* one or multiple SECONDARY Low-Noise STEMlab 125-14 devices, that are modified in a way that they can receive clock and trigger signals from a PRIMARY device and distribute them to the next SECONDARY device. These are marked with an “S” sticker.

For detailed hardware specifications for Low-Noise STEMlab 125-14 devices used in the STEMlab 125-14 X-Channel System, please refer to the :ref:`STEMlab 125-14 standard specs <top_125_14>`.

For more information about the software, please refer to: :ref:`X-Channel streaming <x-ch_streaming>`.

.. note::

    The comparison between :ref:`Red Pitaya X-Channel System and Red Pitaya Click Shield Synchronisation is available here <click_shield_Q&A>`.


Pinout
===========

.. figure:: ../125-14/img/Red_Pitaya_pinout.jpg
    :width: 700


Technical specifications (one board)
------------------------------------

.. table::
    :widths: 20 20

    +------------------------------------+------------------------------------+
    | **Basic**                                                               |
    +====================================+====================================+
    | Processor                          | DUAL CORE ARM CORTEX A9            |
    +------------------------------------+------------------------------------+
    | FPGA                               | FPGA Xilinx Zynq 7010 SOC          |
    +------------------------------------+------------------------------------+
    | RAM                                | 512 MB (4 Gb)                      |
    +------------------------------------+------------------------------------+
    | System memory                      | Micro SD up to 32 GB               |
    +------------------------------------+------------------------------------+
    | Console connection                 | Micro USB                          |
    +------------------------------------+------------------------------------+
    | Power connector                    | Micro USB                          |
    |                                    |                                    |
    +------------------------------------+------------------------------------+
    | Power consumption                  | 5 V, 2 A max                       |
    +------------------------------------+------------------------------------+

|

.. table::
    :widths: 20 20

    +------------------------------------+------------------------------------+
    | **Connectivity**                                                        |
    +====================================+====================================+
    | Ethernet                           | 1 Gbit                             |
    +------------------------------------+------------------------------------+
    | USB                                | USB 2.0                            |
    +------------------------------------+------------------------------------+
    | Wi-Fi                              | requires Wi-Fi dongle              |
    +------------------------------------+------------------------------------+

|

.. table::
    :widths: 20 20

    +------------------------------------+------------------------------------+
    | **RF inputs**                                                           |
    +====================================+====================================+
    | RF input channels                  | 2                                  |
    +------------------------------------+------------------------------------+
    | Sample rate                        | 125 MS/s                           |
    +------------------------------------+------------------------------------+
    | ADC resolution                     | 14 bit                             |
    +------------------------------------+------------------------------------+
    | Input impedance                    | 1 MΩ / 10 pF                       |
    +------------------------------------+------------------------------------+
    | Full scale voltage range           | ±1 V (LV) and ±20 V (HV)           |
    +------------------------------------+------------------------------------+
    | Input coupling                     | DC                                 |
    +------------------------------------+------------------------------------+
    | Absolute max. Input voltage range  | 30 V                               |
    |                                    |                                    |
    +------------------------------------+------------------------------------+
    | Input ESD protection               | Yes                                |
    +------------------------------------+------------------------------------+
    | Overload protection                | Protection diodes                  |
    +------------------------------------+------------------------------------+
    | Bandwidth                          | DC - 60 MHz                        |
    +------------------------------------+------------------------------------+

|

.. table::
    :widths: 20 20

    +------------------------------------+------------------------------------+
    | **RF outputs**                                                          |
    +====================================+====================================+
    | RF output channels                 | 2                                  |
    +------------------------------------+------------------------------------+
    | Sample rate                        | 125 MS/s                           |
    +------------------------------------+------------------------------------+
    | DAC resolution                     | 14 bit                             |
    +------------------------------------+------------------------------------+
    | Load impedance                     | 50 Ω                               |
    +------------------------------------+------------------------------------+
    | Voltage range                      | ±1 V                               |
    |                                    |                                    |
    +------------------------------------+------------------------------------+
    | Short circuit protection           | Yes                                |
    |                                    |                                    |
    +------------------------------------+------------------------------------+
    | Connector type                     | SMA                                |
    +------------------------------------+------------------------------------+
    | Output slew rate                   | 2 V / 10 ns                        |
    +------------------------------------+------------------------------------+
    | Bandwidth                          | DC - 50 MHz                        |
    +------------------------------------+------------------------------------+

|

.. table::
    :widths: 20 20

    +------------------------------------+------------------------------------+
    | **Extension connector**                                                 | 
    +====================================+====================================+
    | Digital IOs                        | 22                                 |
    +------------------------------------+------------------------------------+
    | Analog inputs                      | 4                                  |
    +------------------------------------+------------------------------------+
    | Analog inputs voltage range        | 0-3.5 V                            |
    +------------------------------------+------------------------------------+
    | Sample rate                        | 100 kS/s                           |
    +------------------------------------+------------------------------------+
    | Resolution                         | 12 bit                             |
    +------------------------------------+------------------------------------+
    | Analog outputs                     | 4                                  |
    +------------------------------------+------------------------------------+
    | Analog outputs voltage range       | 0-1.8 V                            |
    +------------------------------------+------------------------------------+
    | Communication interfaces           | I2C, SPI, UART, CAN                |
    +------------------------------------+------------------------------------+
    | Available voltages                 | +5 V, +3.3 V, -4 V                 |
    +------------------------------------+------------------------------------+
    | External ADC clock                 |  Yes                               |
    +------------------------------------+------------------------------------+

|

.. table::
    :widths: 20 20

    +------------------------------------+------------------------------------+
    | **Synchronisation**                                                     |
    +====================================+====================================+
    | Trigger input                      | Through extension connector        |
    +------------------------------------+------------------------------------+
    | Daisy chain connection             | Over SATA connection               |
    |                                    | (up to 500 Mbps)                   |
    +------------------------------------+------------------------------------+
    | Ref. clock input                   | N/A                                |
    +------------------------------------+------------------------------------+

|

.. table::
    :widths: 20 40

    +------------------------------------+-------------------------------------------+
    | **More**                                                                       |
    +====================================+===========================================+
    | Options                            | 4-Ch IN + 4-Ch OUT                        |
    |                                    +-------------------------------------------+
    |                                    | 6-Ch IN + 6-Ch OUT                        |
    |                                    +-------------------------------------------+
    |                                    | (2*x)-Ch IN + (2*x)-Ch OUT; (3 < x < 8)   |
    |                                    +-------------------------------------------+
    |                                    | 16-Ch IN + 16-Ch OUT                      |
    +------------------------------------+-------------------------------------------+


.. note::

    For more information, please refer to the :ref:`Product comparison table <rp-board-comp>` and :ref:`STEMlab 125-14 Low-Noise <top_125_14_LN>`.



Other specifications
=====================

For all other specifications please refer to standard :ref:`STEMlab 125-14 specs <top_125_14>`.

