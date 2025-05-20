# Struct: <code>pci_vpd</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pci_vpd {
    unsigned int len;
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    u8 busy;
    u8 valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    u8 busy;
    u8 valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    u8 busy;
    u8 valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    u8 busy;
    u8 valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pci_vpd {
    struct mutex lock;
    unsigned int len;
    u8 cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pci_vpd {
    struct mutex lock;
    unsigned int len;
    u8 cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pci_vpd {
    struct mutex lock;
    unsigned int len;
    u8 cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pci_vpd {
    struct mutex lock;
    unsigned int len;
    u8 cap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pci_vpd {
    struct mutex lock;
    unsigned int len;
    u8 cap;
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
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
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
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pci_vpd {
    const struct pci_vpd_ops *ops;
    struct bin_attribute *attr;
    struct mutex lock;
    unsigned int len;
    u16 flag;
    u8 cap;
    unsigned int busy;
    unsigned int valid;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex lock</code>
</li>
<li>
<b>Field added. </b>
<code>u16 flag</code>
</li>
<li>
<b>Field added. </b>
<code>u8 cap</code>
</li>
<li>
<b>Field added. </b>
<code>u8 busy</code>
</li>
<li>
<b>Field added. </b>
<code>u8 valid</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 busy</code> ➡️ <code>unsigned int busy</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 valid</code> ➡️ <code>unsigned int valid</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct bin_attribute *attr</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>const struct pci_vpd_ops *ops</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 flag</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int busy</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int valid</code>
</li>
</ul>
</details>
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
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
