# Struct: <code>nand_jedec_params</code>

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
struct nand_jedec_params {
    u8 sig[4];
    __le16 revision;
    __le16 features;
    u8 opt_cmd[3];
    __le16 sec_cmd;
    u8 num_of_param_pages;
    u8 reserved0[18];
    char manufacturer[12];
    char model[20];
    u8 jedec_id[6];
    u8 reserved1[10];
    __le32 byte_per_page;
    __le16 spare_bytes_per_page;
    u8 reserved2[6];
    __le32 pages_per_block;
    __le32 blocks_per_lun;
    u8 lun_count;
    u8 addr_cycles;
    u8 bits_per_cell;
    u8 programs_per_page;
    u8 multi_plane_addr;
    u8 multi_plane_op_attr;
    u8 reserved3[38];
    __le16 async_sdr_speed_grade;
    __le16 toggle_ddr_speed_grade;
    __le16 sync_ddr_speed_grade;
    u8 async_sdr_features;
    u8 toggle_ddr_features;
    u8 sync_ddr_features;
    __le16 t_prog;
    __le16 t_bers;
    __le16 t_r;
    __le16 t_r_multi_plane;
    __le16 t_ccs;
    __le16 io_pin_capacitance_typ;
    __le16 input_pin_capacitance_typ;
    __le16 clk_pin_capacitance_typ;
    u8 driver_strength_support;
    __le16 t_adl;
    u8 reserved4[36];
    u8 guaranteed_good_blocks;
    __le16 guaranteed_block_endurance;
    struct jedec_ecc_info ecc_info[4];
    u8 reserved5[29];
    u8 reserved6[148];
    __le16 vendor_rev_num;
    u8 reserved7[88];
    __le16 crc;
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
