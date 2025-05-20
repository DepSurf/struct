# Struct: <code>cper_sec_proc_arm</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    __u32 validation_bits;
    __u16 err_info_num;
    __u16 context_info_num;
    __u32 section_length;
    __u8 affinity_level;
    __u8 reserved[3];
    __u64 mpidr;
    __u64 midr;
    __u32 running_state;
    __u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    __u32 validation_bits;
    __u16 err_info_num;
    __u16 context_info_num;
    __u32 section_length;
    __u8 affinity_level;
    __u8 reserved[3];
    __u64 mpidr;
    __u64 midr;
    __u32 running_state;
    __u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    __u32 validation_bits;
    __u16 err_info_num;
    __u16 context_info_num;
    __u32 section_length;
    __u8 affinity_level;
    __u8 reserved[3];
    __u64 mpidr;
    __u64 midr;
    __u32 running_state;
    __u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    __u32 validation_bits;
    __u16 err_info_num;
    __u16 context_info_num;
    __u32 section_length;
    __u8 affinity_level;
    __u8 reserved[3];
    __u64 mpidr;
    __u64 midr;
    __u32 running_state;
    __u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
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
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
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
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cper_sec_proc_arm {
    u32 validation_bits;
    u16 err_info_num;
    u16 context_info_num;
    u32 section_length;
    u8 affinity_level;
    u8 reserved[3];
    u64 mpidr;
    u64 midr;
    u32 running_state;
    u32 psci_state;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>__u32 validation_bits</code> ➡️ <code>u32 validation_bits</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 err_info_num</code> ➡️ <code>u16 err_info_num</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u16 context_info_num</code> ➡️ <code>u16 context_info_num</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 section_length</code> ➡️ <code>u32 section_length</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 affinity_level</code> ➡️ <code>u8 affinity_level</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 reserved[3]</code> ➡️ <code>u8 reserved[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 mpidr</code> ➡️ <code>u64 mpidr</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u64 midr</code> ➡️ <code>u64 midr</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 running_state</code> ➡️ <code>u32 running_state</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 psci_state</code> ➡️ <code>u32 psci_state</code>
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
