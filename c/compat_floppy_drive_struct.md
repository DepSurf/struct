# Struct: <code>compat_floppy_drive_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct compat_floppy_drive_struct {
    signed char flags;
    compat_ulong_t spinup_date;
    compat_ulong_t select_date;
    compat_ulong_t first_read_date;
    short int probed_format;
    short int track;
    short int maxblock;
    short int maxtrack;
    compat_int_t generation;
    compat_int_t keep_data;
    compat_int_t fd_ref;
    compat_int_t fd_device;
    compat_int_t last_checked;
    compat_caddr_t dmabuf;
    compat_int_t bufblocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct compat_floppy_drive_struct {
    signed char flags;
    compat_ulong_t spinup_date;
    compat_ulong_t select_date;
    compat_ulong_t first_read_date;
    short int probed_format;
    short int track;
    short int maxblock;
    short int maxtrack;
    compat_int_t generation;
    compat_int_t keep_data;
    compat_int_t fd_ref;
    compat_int_t fd_device;
    compat_int_t last_checked;
    compat_caddr_t dmabuf;
    compat_int_t bufblocks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct compat_floppy_drive_struct {
    signed char flags;
    compat_ulong_t spinup_date;
    compat_ulong_t select_date;
    compat_ulong_t first_read_date;
    short int probed_format;
    short int track;
    short int maxblock;
    short int maxtrack;
    compat_int_t generation;
    compat_int_t keep_data;
    compat_int_t fd_ref;
    compat_int_t fd_device;
    compat_int_t last_checked;
    compat_caddr_t dmabuf;
    compat_int_t bufblocks;
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
