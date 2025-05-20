# Struct: <code>lpss_private_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct lpss_private_data {
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct lpss_private_data {
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct lpss_private_data {
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct lpss_private_data {
    struct acpi_device *adev;
    void *mmio_base;
    resource_size_t mmio_size;
    unsigned int fixed_clk_rate;
    struct clk *clk;
    const struct lpss_device_desc *dev_desc;
    u32 prv_reg_ctx[9];
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
<code>struct acpi_device *adev</code>
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
</ul>
<b>Flavor</b>
<ul>
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
