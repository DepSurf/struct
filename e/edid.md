# Struct: <code>edid</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
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
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 blue_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
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
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
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
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct edid {
    u8 header[8];
    u8 mfg_id[2];
    u8 prod_code[2];
    u32 serial;
    u8 mfg_week;
    u8 mfg_year;
    u8 version;
    u8 revision;
    u8 input;
    u8 width_cm;
    u8 height_cm;
    u8 gamma;
    u8 features;
    u8 red_green_lo;
    u8 black_white_lo;
    u8 red_x;
    u8 red_y;
    u8 green_x;
    u8 green_y;
    u8 blue_x;
    u8 blue_y;
    u8 white_x;
    u8 white_y;
    struct est_timings established_timings;
    struct std_timing standard_timings[8];
    struct detailed_timing detailed_timings[4];
    u8 extensions;
    u8 checksum;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
