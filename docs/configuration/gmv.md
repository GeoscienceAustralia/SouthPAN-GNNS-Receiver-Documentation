---
layout: default
title: GMV
parent: Receiver Configuration
has_children: false
---

# GMV
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

## MagicUT

The MagicUT receiver can be configured through the device's Android interface.

### L1 SBAS {#magicut-l1sbas}

1. On the home screen, open the **MagicSBAS** application.

2. Press the **settings icon** at the bottom of the screen, then select **SBAS receiver settings**.

3. Set the following options:

    ```text
    SBAS Augmentation PRN: 122
    SBAS Augmentation Mode: SBAS L1 or SBAS Enabled L1*
    SBAS Corrections Source: SBAS through GEO
    ```

    \* SBAS Enabled L1 is a mixed solution which uses the SBAS L1 information for accuracy when it is available. This solution is focused on increasing the availability and accuracy of the position computation in environments with degraded satellite visibility. No integrity is computed in this solution.
    {: .fs-1 }

### DFMC {#magicut-dfmc}

1. On the home screen, open the **MagicSBAS** application.

2. Press the **settings icon** at the bottom of the screen, then select **SBAS receiver settings**.

3. Set the following options:

    ```text
    SBAS Augmentation PRN: 122
    SBAS Augmentation Mode: SBAS DFMC or SBAS Enabled DFMC*
    SBAS Corrections Source: SBAS through GEO
    ```

    \* SBAS Enabled DFMC is a mixed solution which uses the SBAS DFMC information for accuracy when it is available. This solution is focused on increasing the availability and accuracy of the position computation in environments with degraded satellite visibility. No integrity is computed in this solution.
    {: .fs-1 }

### PVS {#magicut-pvs}

1. On the home screen, open the **MagicPPP** application.

2. Press the **menu icon** at the top-left of the screen, then select **Settings**.

3. Set the following options:

    ```text
    Corrections Source: SBAS GEO
    ```
