# Struct: <code>sdma_script_start_addrs</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
In <code>4.8</code>: Absent ⚠️
</li>
<li>
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sdma_script_start_addrs {
    s32 ap_2_ap_addr;
    s32 ap_2_bp_addr;
    s32 ap_2_ap_fixed_addr;
    s32 bp_2_ap_addr;
    s32 loopback_on_dsp_side_addr;
    s32 mcu_interrupt_only_addr;
    s32 firi_2_per_addr;
    s32 firi_2_mcu_addr;
    s32 per_2_firi_addr;
    s32 mcu_2_firi_addr;
    s32 uart_2_per_addr;
    s32 uart_2_mcu_addr;
    s32 per_2_app_addr;
    s32 mcu_2_app_addr;
    s32 per_2_per_addr;
    s32 uartsh_2_per_addr;
    s32 uartsh_2_mcu_addr;
    s32 per_2_shp_addr;
    s32 mcu_2_shp_addr;
    s32 ata_2_mcu_addr;
    s32 mcu_2_ata_addr;
    s32 app_2_per_addr;
    s32 app_2_mcu_addr;
    s32 shp_2_per_addr;
    s32 shp_2_mcu_addr;
    s32 mshc_2_mcu_addr;
    s32 mcu_2_mshc_addr;
    s32 spdif_2_mcu_addr;
    s32 mcu_2_spdif_addr;
    s32 asrc_2_mcu_addr;
    s32 ext_mem_2_ipu_addr;
    s32 descrambler_addr;
    s32 dptc_dvfs_addr;
    s32 utra_addr;
    s32 ram_code_start_addr;
    s32 mcu_2_ssish_addr;
    s32 ssish_2_mcu_addr;
    s32 hdmi_dma_addr;
    s32 zcanfd_2_mcu_addr;
    s32 zqspi_2_mcu_addr;
    s32 mcu_2_ecspi_addr;
    s32 mcu_2_zqspi_addr;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Arch</b>
<ul>
</ul>
