---
layout: default
title: Eos Positioning Systems
parent: Receiver Configuration
has_children: false
---

# Eos Positioning Systems
{: .no_toc }

Eos Positioning Systems receivers can be configured with the [Eos Utility](https://eos-gnss.com/products/software/eos-utility) software.

## Arrow Series

{: .receivers }
>
> - Arrow Lite
> - Arrow 100/100+
> - Arrow 200
> - Arrow Gold/Gold+

### L1 SBAS {#arrow-l1sbas}

1. Connect the receiver to a Windows computer via USB cable.

2. In Eos Utility connect to the receiver: **Port &rarr; COMX &rarr; Connect**.

3. Select **Advanced**.

4. In the **RX Config** tab, set the following:

    ```text
    Diff Source: SBAS
    SBAS Ranging Mode: NO
    ```

    - In the right panel under **Diff Includes**, ensure SBAS is enabled.

5. In the **SBAS** tab, set the following:

    ```text
    Mode: Manual
    PRN(1): 122
    PRN(2): 122
    PRN(3): 122
    ```

6. Save settings to receiver memory (if you want settings to persist after reboot): **File &rarr; Save Settings**.
