# Struct: <code>kvm_apic_map</code>

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
struct kvm_apic_map {
    struct callback_head rcu;
    u8 mode;
    u32 max_apic_id;
    struct kvm_lapic * xapic_flat_map[8];
    struct kvm_lapic * xapic_cluster_map[64];
    struct kvm_lapic * phys_map[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_apic_map {
    struct callback_head rcu;
    u8 mode;
    u32 max_apic_id;
    struct kvm_lapic * xapic_flat_map[8];
    struct kvm_lapic * xapic_cluster_map[64];
    struct kvm_lapic * phys_map[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_apic_map {
    struct callback_head rcu;
    u8 mode;
    u32 max_apic_id;
    struct kvm_lapic * xapic_flat_map[8];
    struct kvm_lapic * xapic_cluster_map[64];
    struct kvm_lapic * phys_map[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_apic_map {
    struct callback_head rcu;
    u8 mode;
    u32 max_apic_id;
    struct kvm_lapic * xapic_flat_map[8];
    struct kvm_lapic * xapic_cluster_map[64];
    struct kvm_lapic * phys_map[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_apic_map {
    struct callback_head rcu;
    u8 mode;
    u32 max_apic_id;
    struct kvm_lapic * xapic_flat_map[8];
    struct kvm_lapic * xapic_cluster_map[64];
    struct kvm_lapic * phys_map[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_apic_map {
    struct callback_head rcu;
    enum kvm_apic_logical_mode logical_mode;
    u32 max_apic_id;
    struct kvm_lapic * xapic_flat_map[8];
    struct kvm_lapic * xapic_cluster_map[64];
    struct kvm_lapic * phys_map[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_apic_map {
    struct callback_head rcu;
    enum kvm_apic_logical_mode logical_mode;
    u32 max_apic_id;
    struct kvm_lapic * xapic_flat_map[8];
    struct kvm_lapic * xapic_cluster_map[64];
    struct kvm_lapic * phys_map[0];
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum kvm_apic_logical_mode logical_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 mode</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
