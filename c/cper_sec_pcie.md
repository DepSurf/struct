# Struct: <code>cper_sec_pcie</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cper_sec_pcie {
    __u64 validation_bits;
    __u32 port_type;
    struct (anon) version;
    __u16 command;
    __u16 status;
    __u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    __u8 capability[60];
    __u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cper_sec_pcie {
    __u64 validation_bits;
    __u32 port_type;
    struct (anon) version;
    __u16 command;
    __u16 status;
    __u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    __u8 capability[60];
    __u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cper_sec_pcie {
    __u64 validation_bits;
    __u32 port_type;
    struct (anon) version;
    __u16 command;
    __u16 status;
    __u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    __u8 capability[60];
    __u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cper_sec_pcie {
    __u64 validation_bits;
    __u32 port_type;
    struct (anon) version;
    __u16 command;
    __u16 status;
    __u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    __u8 capability[60];
    __u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cper_sec_pcie {
    __u64 validation_bits;
    __u32 port_type;
    struct (anon) version;
    __u16 command;
    __u16 status;
    __u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    __u8 capability[60];
    __u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cper_sec_pcie {
    __u64 validation_bits;
    __u32 port_type;
    struct (anon) version;
    __u16 command;
    __u16 status;
    __u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    __u8 capability[60];
    __u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cper_sec_pcie {
    __u64 validation_bits;
    __u32 port_type;
    struct (anon) version;
    __u16 command;
    __u16 status;
    __u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    __u8 capability[60];
    __u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
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
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cper_sec_pcie {
    u64 validation_bits;
    u32 port_type;
    struct (anon) version;
    u16 command;
    u16 status;
    u32 reserved;
    struct (anon) device_id;
    struct (anon) serial_number;
    struct (anon) bridge;
    u8 capability[60];
    u8 aer_info[96];
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__u64 validation_bits</code> ➡️ <code>u64 validation_bits</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 port_type</code> ➡️ <code>u32 port_type</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 command</code> ➡️ <code>u16 command</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 status</code> ➡️ <code>u16 status</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 reserved</code> ➡️ <code>u32 reserved</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 capability[60]</code> ➡️ <code>u8 capability[60]</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 aer_info[96]</code> ➡️ <code>u8 aer_info[96]</code>
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
