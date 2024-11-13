---
layout: default
title: u-blox
parent: Receiver Configuration
has_children: false
---

# u-blox
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

## Generation 8 Modules

u-blox Generation 8 Modules can be configured with the [u-center](https://www.u-blox.com/en/product/u-center) software.

{: .receivers }
>
> - CAM-M8 variants
> - EVA-M8 variants
> - LEA-M8 variants
> - MAX-M8 variants
> - NEO-M8 variants
> - ZOE-M8 variants

### L1 SBAS {#generation-8-modules-l1sbas}

1. Connect the u-blox receiver to a Windows computer via USB cable.

2. In u-center connect to the receiver: **Receiver &rarr; Connection &rarr; COMX**.

3. Open the configuration view: **View &rarr; Configuration View**.

4. Scroll down to **GNSS (GNSS Config)** and set the following:

    ```text
    SBAS configure: On
    SBAS enable: On
    ```

    - Click Send message.

5. Scroll down to **SBAS (SBAS Settings)** and set the following:

    ```text
    Subsystem: Enabled
    Allow test mode use (Msg 0): On
    Ranging (Use SBAS in NAV): Off
    Apply SBAS Correction data: On
    Apply integrity information: Off
    Number of search channels: 3
    PRN Codes: Other, 122
    ```

    - Click Send message.

6. Save settings to receiver memory (if you want settings to persist after reboot):

    - Scroll to **CFG (Configuration)**.
    - Click **Save current configuration**.
    - Highlight all devices (`BBR`, `FLASH`, `I2C-EEPROM`, `SPI-FLASH`).
    - Click Send message.

## Generation 9 Modules

u-blox Generation 9 Modules can be configured with the [u-center](https://www.u-blox.com/en/product/u-center) software.

{: .receivers }
>
> - NEO-F9 variants
> - NEO-M9 variants
> - ZED-F9 variants

### L1 SBAS {#generation-9-modules-l1sbas}

1. Connect the u-blox receiver to a Windows computer via USB cable.

2. In u-center connect to the receiver: **Receiver &rarr; Connection &rarr; COMX**.

3. Open the configuration view: **View &rarr; Configuration View**.

4. Scroll down to **GNSS (GNSS Config)** and set the following:

    ```text
    SBAS configure: On
    SBAS enable: On
    ```

    - Click Send message.

5. Scroll down to **SBAS (SBAS Settings)** and set the following:

    ```text
    Subsystem: Enabled
    Allow test mode use (Msg 0): On
    Ranging (Use SBAS in NAV): Off
    Apply SBAS Correction data: On
    Apply integrity information: Off
    Number of search channels: 3
    PRN Codes: Other, 122
    ```

    - Click Send message.

6. Save settings to receiver memory (if you want settings to persist after reboot):

    - Scroll to **CFG (Configuration)**.
    - Click **Save current configuration**.
    - Highlight all devices (`BBR`, `FLASH`, `I2C-EEPROM`, `SPI-FLASH`).
    - Click Send message.

## Generation 10 Modules

u-blox Generation 10 Modules can be configured with the [u-center 2](https://www.u-blox.com/en/u-center-2) software.

{: .receivers }
>
> - MAX-M10 variants
> - MIA-M10 variatns
> - NEO-F10 variants

### L1 SBAS {#generation-10-modules-l1sbas}

1. Connect the u-blox receiver to a Windows computer via USB cable.

2. In u-center connect to the receiver: **Devices &rarr; Add device &rarr; Select COM port &rarr; COMX**.

3. Open the configuration menu: **Devices &rarr; Device configuration**.

4. Scroll down to **CFG-SIGNAL (GNSS Signal Config)** and set the following:

    ```text
    CFG-SIGNAL-SBAS_ENA: 1, True
    CFG-SIGNAL-SBAS_L1CA_ENA : 1, True
    ```

    - Write each setting to layer **RAM** (Also set **BBR** and/or **Flash** for settings to persist after reboot).
    - Click Send.

5. Scroll to **CFG-SBAS (SBAS Config)** and set the following:

    ```text
    CFG-SBAS-USE_TESTMODE: 1, True
    CFG-SBAS-USE_RANGING: 0, False
    CFG-SBAS-USE_DIFFCORR: 1, True
    CFG-SBAS-USE_INTEGRITY: 0, False
    CFG-SBAS-PRNSCANMASK: 4 (Enable search for SBAS PRN122)
    ```

    - Write each setting to layer **RAM** (Also set **BBR** and/or **Flash** for settings to persist after reboot).
    - Click Send.
