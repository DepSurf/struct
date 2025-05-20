# Struct: <code>dpc_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    struct work_struct work;
    int cap_pos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    struct work_struct work;
    int cap_pos;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    struct work_struct work;
    int cap_pos;
    bool rp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    struct work_struct work;
    int cap_pos;
    bool rp;
    u32 rp_pio_status;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    struct work_struct work;
    u16 cap_pos;
    bool rp_extensions;
    u32 rp_pio_status;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
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
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
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
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dpc_dev {
    struct pcie_device *dev;
    u16 cap_pos;
    bool rp_extensions;
    u8 rp_log_size;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool rp</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 rp_pio_status</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool rp_extensions</code>
</li>
<li>
<b>Field added. </b>
<code>u8 rp_log_size</code>
</li>
<li>
<b>Field removed. </b>
<code>bool rp</code>
</li>
<li>
<b>Field type changed. </b>
<code>int cap_pos</code> ➡️ <code>u16 cap_pos</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct work_struct work</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rp_pio_status</code>
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
