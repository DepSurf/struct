# Struct: <code>kvm_memory_slot</code>

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
struct kvm_memory_slot {
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
    u16 as_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_memory_slot {
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
    u16 as_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_memory_slot {
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
    u16 as_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_memory_slot {
    struct hlist_node id_node[2];
    struct interval_tree_node hva_node[2];
    struct rb_node gfn_node[2];
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
    u16 as_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_memory_slot {
    struct hlist_node id_node[2];
    struct interval_tree_node hva_node[2];
    struct rb_node gfn_node[2];
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
    u16 as_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_memory_slot {
    struct hlist_node id_node[2];
    struct interval_tree_node hva_node[2];
    struct rb_node gfn_node[2];
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
    u16 as_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_memory_slot {
    struct hlist_node id_node[2];
    struct interval_tree_node hva_node[2];
    struct rb_node gfn_node[2];
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
    u16 as_id;
    struct (anon) gmem;
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
struct kvm_memory_slot {
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kvm_memory_slot {
    gfn_t base_gfn;
    long unsigned int npages;
    long unsigned int *dirty_bitmap;
    struct kvm_arch_memory_slot arch;
    long unsigned int userspace_addr;
    u32 flags;
    short int id;
};
```
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node id_node[2]</code>
</li>
<li>
<b>Field added. </b>
<code>struct interval_tree_node hva_node[2]</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_node gfn_node[2]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct (anon) gmem</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
