# Struct: <code>floppy_fdc_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct floppy_fdc_state {
    int spec1;
    int spec2;
    int dtr;
    unsigned char version;
    unsigned char dor;
    long unsigned int address;
    unsigned int rawcmd;
    unsigned int reset;
    unsigned int need_configure;
    unsigned int perp_mode;
    unsigned int has_fifo;
    unsigned int driver_version;
    unsigned char track[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct floppy_fdc_state {
    int spec1;
    int spec2;
    int dtr;
    unsigned char version;
    unsigned char dor;
    long unsigned int address;
    unsigned int rawcmd;
    unsigned int reset;
    unsigned int need_configure;
    unsigned int perp_mode;
    unsigned int has_fifo;
    unsigned int driver_version;
    unsigned char track[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct floppy_fdc_state {
    int spec1;
    int spec2;
    int dtr;
    unsigned char version;
    unsigned char dor;
    long unsigned int address;
    unsigned int rawcmd;
    unsigned int reset;
    unsigned int need_configure;
    unsigned int perp_mode;
    unsigned int has_fifo;
    unsigned int driver_version;
    unsigned char track[4];
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
