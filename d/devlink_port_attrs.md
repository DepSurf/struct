# Struct: <code>devlink_port_attrs</code>

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
struct devlink_port_attrs {
    bool set;
    enum devlink_port_flavour flavour;
    u32 port_number;
    bool split;
    u32 split_subport_number;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct devlink_port_attrs {
    bool set;
    enum devlink_port_flavour flavour;
    u32 port_number;
    bool split;
    u32 split_subport_number;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 split;
    u8 splittable;
    u32 lanes;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 split;
    u8 splittable;
    u32 lanes;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
    struct devlink_port_pci_sf_attrs pci_sf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 split;
    u8 splittable;
    u32 lanes;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
    struct devlink_port_pci_sf_attrs pci_sf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 split;
    u8 splittable;
    u32 lanes;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
    struct devlink_port_pci_sf_attrs pci_sf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 split;
    u8 splittable;
    u32 lanes;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
    struct devlink_port_pci_sf_attrs pci_sf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 split;
    u8 splittable;
    u32 lanes;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
    struct devlink_port_pci_sf_attrs pci_sf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 split;
    u8 splittable;
    u32 lanes;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
    struct devlink_port_pci_sf_attrs pci_sf;
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
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
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
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct devlink_port_attrs {
    u8 set;
    u8 split;
    u8 switch_port;
    enum devlink_port_flavour flavour;
    struct netdev_phys_item_id switch_id;
    struct devlink_port_phys_attrs phys;
    struct devlink_port_pci_pf_attrs pci_pf;
    struct devlink_port_pci_vf_attrs pci_vf;
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 switch_port</code>
</li>
<li>
<b>Field added. </b>
<code>struct netdev_phys_item_id switch_id</code>
</li>
<li>
<b>Field added. </b>
<code>struct devlink_port_phys_attrs phys</code>
</li>
<li>
<b>Field added. </b>
<code>struct devlink_port_pci_pf_attrs pci_pf</code>
</li>
<li>
<b>Field added. </b>
<code>struct devlink_port_pci_vf_attrs pci_vf</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 port_number</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 split_subport_number</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool set</code> ➡️ <code>u8 set</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool split</code> ➡️ <code>u8 split</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 splittable</code>
</li>
<li>
<b>Field added. </b>
<code>u32 lanes</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 set</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 switch_port</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct devlink_port_pci_sf_attrs pci_sf</code>
</li>
</ul>
</details>
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
