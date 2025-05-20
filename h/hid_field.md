# Struct: <code>hid_field</code>

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
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hid_field {
    unsigned int physical;
    unsigned int logical;
    unsigned int application;
    struct hid_usage *usage;
    unsigned int maxusage;
    unsigned int flags;
    unsigned int report_offset;
    unsigned int report_size;
    unsigned int report_count;
    unsigned int report_type;
    __s32 *value;
    __s32 *new_value;
    __s32 *usages_priorities;
    __s32 logical_minimum;
    __s32 logical_maximum;
    __s32 physical_minimum;
    __s32 physical_maximum;
    __s32 unit_exponent;
    unsigned int unit;
    bool ignored;
    struct hid_report *report;
    unsigned int index;
    struct hid_input *hidinput;
    __u16 dpad;
    unsigned int slot_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hid_field {
    unsigned int physical;
    unsigned int logical;
    unsigned int application;
    struct hid_usage *usage;
    unsigned int maxusage;
    unsigned int flags;
    unsigned int report_offset;
    unsigned int report_size;
    unsigned int report_count;
    unsigned int report_type;
    __s32 *value;
    __s32 *new_value;
    __s32 *usages_priorities;
    __s32 logical_minimum;
    __s32 logical_maximum;
    __s32 physical_minimum;
    __s32 physical_maximum;
    __s32 unit_exponent;
    unsigned int unit;
    bool ignored;
    struct hid_report *report;
    unsigned int index;
    struct hid_input *hidinput;
    __u16 dpad;
    unsigned int slot_idx;
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
