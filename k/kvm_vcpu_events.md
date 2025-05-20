# Struct: <code>kvm_vcpu_events</code>

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
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kvm_vcpu_events {
    struct (anon) exception;
    struct (anon) interrupt;
    struct (anon) nmi;
    __u32 sipi_vector;
    __u32 flags;
    struct (anon) smi;
    __u8 reserved[27];
    __u8 exception_has_payload;
    __u64 exception_payload;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_vcpu_events {
    struct (anon) exception;
    struct (anon) interrupt;
    struct (anon) nmi;
    __u32 sipi_vector;
    __u32 flags;
    struct (anon) smi;
    __u8 reserved[27];
    __u8 exception_has_payload;
    __u64 exception_payload;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_vcpu_events {
    struct (anon) exception;
    struct (anon) interrupt;
    struct (anon) nmi;
    __u32 sipi_vector;
    __u32 flags;
    struct (anon) smi;
    __u8 reserved[27];
    __u8 exception_has_payload;
    __u64 exception_payload;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_vcpu_events {
    struct (anon) exception;
    struct (anon) interrupt;
    struct (anon) nmi;
    __u32 sipi_vector;
    __u32 flags;
    struct (anon) smi;
    __u8 reserved[27];
    __u8 exception_has_payload;
    __u64 exception_payload;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_vcpu_events {
    struct (anon) exception;
    struct (anon) interrupt;
    struct (anon) nmi;
    __u32 sipi_vector;
    __u32 flags;
    struct (anon) smi;
    struct (anon) triple_fault;
    __u8 reserved[26];
    __u8 exception_has_payload;
    __u64 exception_payload;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_vcpu_events {
    struct (anon) exception;
    struct (anon) interrupt;
    struct (anon) nmi;
    __u32 sipi_vector;
    __u32 flags;
    struct (anon) smi;
    struct (anon) triple_fault;
    __u8 reserved[26];
    __u8 exception_has_payload;
    __u64 exception_payload;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_vcpu_events {
    struct (anon) exception;
    struct (anon) interrupt;
    struct (anon) nmi;
    __u32 sipi_vector;
    __u32 flags;
    struct (anon) smi;
    struct (anon) triple_fault;
    __u8 reserved[26];
    __u8 exception_has_payload;
    __u64 exception_payload;
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
struct kvm_vcpu_events {
    struct (anon) exception;
    __u32 reserved[12];
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) triple_fault</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 reserved[27]</code> ➡️ <code>__u8 reserved[26]</code>
</li>
</ul>
</details>
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
