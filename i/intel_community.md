# Struct: <code>intel_community</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int pin_base;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    size_t npins;
    unsigned int features;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    void *regs;
    void *pad_regs;
};
```
</details>
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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    size_t npins;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    short unsigned int nirqs;
    short unsigned int acpi_space_id;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    short unsigned int nirqs;
    short unsigned int acpi_space_id;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    short unsigned int nirqs;
    short unsigned int acpi_space_id;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    short unsigned int nirqs;
    short unsigned int acpi_space_id;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    short unsigned int nirqs;
    short unsigned int acpi_space_id;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    short unsigned int nirqs;
    short unsigned int acpi_space_id;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    size_t npins;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    short unsigned int nirqs;
    short unsigned int acpi_space_id;
    void *regs;
    void *pad_regs;
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
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    size_t npins;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    size_t npins;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    size_t npins;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct intel_community {
    unsigned int barno;
    unsigned int padown_offset;
    unsigned int padcfglock_offset;
    unsigned int hostown_offset;
    unsigned int is_offset;
    unsigned int ie_offset;
    unsigned int features;
    unsigned int pin_base;
    unsigned int gpp_size;
    unsigned int gpp_num_padown_regs;
    size_t npins;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    const unsigned int *pad_map;
    void *regs;
    void *pad_regs;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>short unsigned int nirqs</code>
</li>
<li>
<b>Field added. </b>
<code>short unsigned int acpi_space_id</code>
</li>
</ul>
</details>
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
