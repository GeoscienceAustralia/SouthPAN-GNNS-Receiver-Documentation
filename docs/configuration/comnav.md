---
layout: default
title: ComNav
parent: Receiver Configuration
has_children: false
---

# ComNav
{: .no_toc }

## SinoGNSS G100

The SinoGNSS G100 receiver can be configured with the [Compass Receiver Utility](https://www.comnavtech.com/Software.html) software.

### L1 SBAS {#sinognss-g100-l1sbas}

1. Connect the receiver to a Windows computer via Bluetooth or the supplied data cable and a RS232 USB adapter.

2. In Compass Receiver Utility connect to the receiver: **Set Port &rarr; Serial Port &rarr; COMX**.

3. Open the command window: **Receiver &rarr; Command**.

4. Enter the following commands into the text window and press **Send**:

    ```text
    sbascontrol enable 122
    saveconfig
    ```
