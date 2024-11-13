---
layout: default
title: Septentrio
parent: Receiver Configuration
has_children: false
---

# Septentrio

## Mosaic-X5

The Mosaic-X5 can be configured through the web interface, which can be accessed after connecting the receiver to your computer using a USB cable and visiting the IP address [192.168.3.1](http://192.168.3.1) in a browser.

### L1 SBAS {#mosaic-x5-sbas-l1}

1. Connect the receiver to a computer via USB cable and visit the web interface at "192.168.3.1" in a browser.

2. Open the Position view: **GNSS &rarr; Position** and ensure that the **SBAS** position mode is enabled.

3. Open the Control Panel: **Admin &rarr; Expert Control &rarr; Control Panel**.

4. Navigate to the SBAS Corrections options: **Navigation &rarr; Positioning Mode &rarr; SBAS Corrections**, and set the following:

    ```text
    Satellite: S122
    SIS mode: Test
    Navigation mode: MixedSystems
    DO229 version: auto
    ```

    - Click Ok.

5. Press **Save** in the pop-up to save the settings to receiver memory (if you want settings to persist after reboot).
