# Struct: <code>iommu_gpasid_bind_data</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iommu_gpasid_bind_data {
    __u32 version;
    __u32 format;
    __u64 flags;
    __u64 gpgd;
    __u64 hpasid;
    __u64 gpasid;
    __u32 addr_width;
    __u8 padding[12];
    struct iommu_gpasid_bind_data_vtd vtd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iommu_gpasid_bind_data {
    __u32 argsz;
    __u32 version;
    __u32 format;
    __u32 addr_width;
    __u64 flags;
    __u64 gpgd;
    __u64 hpasid;
    __u64 gpasid;
    __u8 padding[8];
    union (anon) vendor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iommu_gpasid_bind_data {
    __u32 argsz;
    __u32 version;
    __u32 format;
    __u32 addr_width;
    __u64 flags;
    __u64 gpgd;
    __u64 hpasid;
    __u64 gpasid;
    __u8 padding[8];
    union (anon) vendor;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iommu_gpasid_bind_data {
    __u32 argsz;
    __u32 version;
    __u32 format;
    __u32 addr_width;
    __u64 flags;
    __u64 gpgd;
    __u64 hpasid;
    __u64 gpasid;
    __u8 padding[8];
    union (anon) vendor;
};
```
</details>
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u32 argsz</code>
</li>
<li>
<b>Field added. </b>
<code>union (anon) vendor</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iommu_gpasid_bind_data_vtd vtd</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 padding[12]</code> ➡️ <code>__u8 padding[8]</code>
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
</ul>
