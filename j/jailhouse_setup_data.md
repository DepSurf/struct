# Struct: <code>jailhouse_setup_data</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    struct (anon) hdr;
    struct (anon) v1;
    struct (anon) v2;
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
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct jailhouse_setup_data {
    __u16 version;
    __u16 compatible_version;
    __u16 pm_timer_address;
    __u16 num_cpus;
    __u64 pci_mmconfig_base;
    __u32 tsc_khz;
    __u32 apic_khz;
    __u8 standard_ioapic;
    __u8 cpu_ids[255];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) hdr</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) v1</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) v2</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 version</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 compatible_version</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 pm_timer_address</code>
</li>
<li>
<b>Field removed. </b>
<code>__u16 num_cpus</code>
</li>
<li>
<b>Field removed. </b>
<code>__u64 pci_mmconfig_base</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 tsc_khz</code>
</li>
<li>
<b>Field removed. </b>
<code>__u32 apic_khz</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 standard_ioapic</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 cpu_ids[255]</code>
</li>
</ul>
</details>
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
