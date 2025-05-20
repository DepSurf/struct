# Struct: <code>nand_onfi_params</code>

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
struct nand_onfi_params {
    u8 sig[4];
    __le16 revision;
    __le16 features;
    __le16 opt_cmd;
    u8 reserved0[2];
    __le16 ext_param_page_length;
    u8 num_of_param_pages;
    u8 reserved1[17];
    char manufacturer[12];
    char model[20];
    u8 jedec_id;
    __le16 date_code;
    u8 reserved2[13];
    __le32 byte_per_page;
    __le16 spare_bytes_per_page;
    __le32 data_bytes_per_ppage;
    __le16 spare_bytes_per_ppage;
    __le32 pages_per_block;
    __le32 blocks_per_lun;
    u8 lun_count;
    u8 addr_cycles;
    u8 bits_per_cell;
    __le16 bb_per_lun;
    __le16 block_endurance;
    u8 guaranteed_good_blocks;
    __le16 guaranteed_block_endurance;
    u8 programs_per_page;
    u8 ppage_attr;
    u8 ecc_bits;
    u8 interleaved_bits;
    u8 interleaved_ops;
    u8 reserved3[13];
    u8 io_pin_capacitance_max;
    __le16 async_timing_mode;
    __le16 program_cache_timing_mode;
    __le16 t_prog;
    __le16 t_bers;
    __le16 t_r;
    __le16 t_ccs;
    __le16 src_sync_timing_mode;
    u8 src_ssync_features;
    __le16 clk_pin_capacitance_typ;
    __le16 io_pin_capacitance_typ;
    __le16 input_pin_capacitance_typ;
    u8 input_pin_capacitance_max;
    u8 driver_strength_support;
    __le16 t_int_r;
    __le16 t_adl;
    u8 reserved4[8];
    __le16 vendor_revision;
    u8 vendor[88];
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
