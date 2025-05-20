# Struct: <code>pci_sriov</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    struct mutex lock;
    resource_size_t barsz[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    struct mutex lock;
    resource_size_t barsz[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    struct mutex lock;
    resource_size_t barsz[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 cfg_size;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
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
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
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
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pci_sriov {
    int pos;
    int nres;
    u32 cap;
    u16 ctrl;
    u16 total_VFs;
    u16 initial_VFs;
    u16 num_VFs;
    u16 offset;
    u16 stride;
    u16 vf_device;
    u32 pgsz;
    u8 link;
    u8 max_VF_buses;
    u16 driver_max_VFs;
    struct pci_dev *dev;
    struct pci_dev *self;
    u32 class;
    u8 hdr_type;
    u16 subsystem_vendor;
    u16 subsystem_device;
    resource_size_t barsz[6];
    bool drivers_autoprobe;
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
<code>bool drivers_autoprobe</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex lock</code>
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
<code>u16 vf_device</code>
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
<code>u32 class</code>
</li>
<li>
<b>Field added. </b>
<code>u8 hdr_type</code>
</li>
<li>
<b>Field added. </b>
<code>u16 subsystem_vendor</code>
</li>
<li>
<b>Field added. </b>
<code>u16 subsystem_device</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 cfg_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u32 cfg_size</code>
</li>
</ul>
</details>
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
