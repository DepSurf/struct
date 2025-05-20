# Struct: <code>ghes</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_status *estatus;
    u64 buffer_paddr;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_status *estatus;
    u64 buffer_paddr;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_status *estatus;
    u64 buffer_paddr;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    u64 buffer_paddr;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    u64 buffer_paddr;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    u64 buffer_paddr;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
    struct device *dev;
    struct list_head elist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
    struct device *dev;
    struct list_head elist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
    struct device *dev;
    struct list_head elist;
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
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ghes {
    struct acpi_hest_generic *generic;
    struct acpi_hest_generic_v2 *generic_v2;
    struct acpi_hest_generic_status *estatus;
    long unsigned int flags;
    struct list_head list;
    struct timer_list timer;
    unsigned int irq;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct acpi_hest_generic_v2 *generic_v2</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 buffer_paddr</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device *dev</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head elist</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
