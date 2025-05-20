# Struct: <code>cec_log_addrs</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
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
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
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
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cec_log_addrs {
    __u8 log_addr[4];
    __u16 log_addr_mask;
    __u8 cec_version;
    __u8 num_log_addrs;
    __u32 vendor_id;
    __u32 flags;
    char osd_name[15];
    __u8 primary_device_type[4];
    __u8 log_addr_type[4];
    __u8 all_device_types[4];
    __u8 features[48];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
