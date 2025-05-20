# Struct: <code>fat_bios_param_block</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fat_bios_param_block {
    u16 fat_sector_size;
    u8 fat_sec_per_clus;
    u16 fat_reserved;
    u8 fat_fats;
    u16 fat_dir_entries;
    u16 fat_sectors;
    u16 fat_fat_length;
    u32 fat_total_sect;
    u8 fat16_state;
    u32 fat16_vol_id;
    u32 fat32_length;
    u32 fat32_root_cluster;
    u16 fat32_info_sector;
    u8 fat32_state;
    u32 fat32_vol_id;
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
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
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
