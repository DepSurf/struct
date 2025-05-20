# Struct: <code>acpi_pcct_hw_reduced_type2</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 doorbell_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address doorbell_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
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
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
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
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_pcct_hw_reduced_type2 {
    struct acpi_subtable_header header;
    u32 platform_interrupt;
    u8 flags;
    u8 reserved;
    u64 base_address;
    u64 length;
    struct acpi_generic_address doorbell_register;
    u64 preserve_mask;
    u64 write_mask;
    u32 latency;
    u32 max_access_rate;
    u16 min_turnaround_time;
    struct acpi_generic_address platform_ack_register;
    u64 ack_preserve_mask;
    u64 ack_write_mask;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 platform_interrupt</code>
</li>
<li>
<b>Field added. </b>
<code>struct acpi_generic_address platform_ack_register</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 doorbell_interrupt</code>
</li>
<li>
<b>Field removed. </b>
<code>struct acpi_generic_address doorbell_ack_register</code>
</li>
</ul>
</details>
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
