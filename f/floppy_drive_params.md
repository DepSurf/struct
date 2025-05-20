# Struct: <code>floppy_drive_params</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct floppy_drive_params {
    signed char cmos;
    long unsigned int max_dtr;
    long unsigned int hlt;
    long unsigned int hut;
    long unsigned int srt;
    long unsigned int spinup;
    long unsigned int spindown;
    unsigned char spindown_offset;
    unsigned char select_delay;
    unsigned char rps;
    unsigned char tracks;
    long unsigned int timeout;
    unsigned char interleave_sect;
    struct floppy_max_errors max_errors;
    char flags;
    char read_track;
    short int autodetect[8];
    int checkfreq;
    int native_format;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct floppy_drive_params {
    signed char cmos;
    long unsigned int max_dtr;
    long unsigned int hlt;
    long unsigned int hut;
    long unsigned int srt;
    long unsigned int spinup;
    long unsigned int spindown;
    unsigned char spindown_offset;
    unsigned char select_delay;
    unsigned char rps;
    unsigned char tracks;
    long unsigned int timeout;
    unsigned char interleave_sect;
    struct floppy_max_errors max_errors;
    char flags;
    char read_track;
    short int autodetect[8];
    int checkfreq;
    int native_format;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct floppy_drive_params {
    signed char cmos;
    long unsigned int max_dtr;
    long unsigned int hlt;
    long unsigned int hut;
    long unsigned int srt;
    long unsigned int spinup;
    long unsigned int spindown;
    unsigned char spindown_offset;
    unsigned char select_delay;
    unsigned char rps;
    unsigned char tracks;
    long unsigned int timeout;
    unsigned char interleave_sect;
    struct floppy_max_errors max_errors;
    char flags;
    char read_track;
    short int autodetect[8];
    int checkfreq;
    int native_format;
};
```
</details>
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
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
</ul>
