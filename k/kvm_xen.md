# Struct: <code>kvm_xen</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_xen {
    bool long_mode;
    bool shinfo_set;
    u8 upcall_vector;
    struct gfn_to_hva_cache shinfo_cache;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_xen {
    bool long_mode;
    u8 upcall_vector;
    gfn_t shinfo_gfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_xen {
    u32 xen_version;
    bool long_mode;
    u8 upcall_vector;
    struct gfn_to_pfn_cache shinfo_cache;
    struct idr evtchn_ports;
    long unsigned int poll_mask[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_xen {
    struct mutex xen_lock;
    u32 xen_version;
    bool long_mode;
    bool runstate_update_flag;
    u8 upcall_vector;
    struct gfn_to_pfn_cache shinfo_cache;
    struct idr evtchn_ports;
    long unsigned int poll_mask[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_xen {
    struct mutex xen_lock;
    u32 xen_version;
    bool long_mode;
    bool runstate_update_flag;
    u8 upcall_vector;
    struct gfn_to_pfn_cache shinfo_cache;
    struct idr evtchn_ports;
    long unsigned int poll_mask[16];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_xen {
    struct mutex xen_lock;
    u32 xen_version;
    bool long_mode;
    bool runstate_update_flag;
    u8 upcall_vector;
    struct gfn_to_pfn_cache shinfo_cache;
    struct idr evtchn_ports;
    long unsigned int poll_mask[64];
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>gfn_t shinfo_gfn</code>
</li>
<li>
<b>Field removed. </b>
<code>bool shinfo_set</code>
</li>
<li>
<b>Field removed. </b>
<code>struct gfn_to_hva_cache shinfo_cache</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 xen_version</code>
</li>
<li>
<b>Field added. </b>
<code>struct gfn_to_pfn_cache shinfo_cache</code>
</li>
<li>
<b>Field added. </b>
<code>struct idr evtchn_ports</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int poll_mask[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>gfn_t shinfo_gfn</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex xen_lock</code>
</li>
<li>
<b>Field added. </b>
<code>bool runstate_update_flag</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int poll_mask[16]</code> ➡️ <code>long unsigned int poll_mask[64]</code>
</li>
</ul>
</details>
</li>
</ul>
