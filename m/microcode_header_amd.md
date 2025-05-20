# Struct: <code>microcode_header_amd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct microcode_header_amd {
    u32 data_code;
    u32 patch_id;
    u16 mc_patch_data_id;
    u8 mc_patch_data_len;
    u8 init_flag;
    u32 mc_patch_data_checksum;
    u32 nb_dev_id;
    u32 sb_dev_id;
    u16 processor_rev_id;
    u8 nb_rev_id;
    u8 sb_rev_id;
    u8 bios_api_rev;
    u8 reserved1[3];
    u32 match_reg[8];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
