# Struct: <code>io_tlb_mem</code>

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
struct io_tlb_mem {
    phys_addr_t start;
    phys_addr_t end;
    long unsigned int nslabs;
    long unsigned int used;
    unsigned int index;
    spinlock_t lock;
    struct dentry *debugfs;
    bool late_alloc;
    struct io_tlb_slot slots[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_tlb_mem {
    phys_addr_t start;
    phys_addr_t end;
    long unsigned int nslabs;
    long unsigned int used;
    unsigned int index;
    spinlock_t lock;
    struct dentry *debugfs;
    bool late_alloc;
    bool force_bounce;
    bool for_alloc;
    struct io_tlb_slot *slots;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_tlb_mem {
    phys_addr_t start;
    phys_addr_t end;
    void *vaddr;
    long unsigned int nslabs;
    long unsigned int used;
    unsigned int index;
    spinlock_t lock;
    struct dentry *debugfs;
    bool late_alloc;
    bool force_bounce;
    bool for_alloc;
    struct io_tlb_slot *slots;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_tlb_mem {
    phys_addr_t start;
    phys_addr_t end;
    void *vaddr;
    long unsigned int nslabs;
    long unsigned int used;
    struct dentry *debugfs;
    bool late_alloc;
    bool force_bounce;
    bool for_alloc;
    unsigned int nareas;
    unsigned int area_nslabs;
    struct io_tlb_area *areas;
    struct io_tlb_slot *slots;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_tlb_mem {
    phys_addr_t start;
    phys_addr_t end;
    void *vaddr;
    long unsigned int nslabs;
    struct dentry *debugfs;
    bool late_alloc;
    bool force_bounce;
    bool for_alloc;
    unsigned int nareas;
    unsigned int area_nslabs;
    struct io_tlb_area *areas;
    struct io_tlb_slot *slots;
    atomic_long_t total_used;
    atomic_long_t used_hiwater;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_tlb_mem {
    struct io_tlb_pool defpool;
    long unsigned int nslabs;
    struct dentry *debugfs;
    bool force_bounce;
    bool for_alloc;
    bool can_grow;
    u64 phys_limit;
    spinlock_t lock;
    struct list_head pools;
    struct work_struct dyn_alloc;
    atomic_long_t total_used;
    atomic_long_t used_hiwater;
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
<code>bool force_bounce</code>
</li>
<li>
<b>Field added. </b>
<code>bool for_alloc</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct io_tlb_slot slots[0]</code> ➡️ <code>struct io_tlb_slot *slots</code>
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
<code>void *vaddr</code>
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
<code>unsigned int nareas</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int area_nslabs</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_tlb_area *areas</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int index</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_long_t total_used</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t used_hiwater</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int used</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct io_tlb_pool defpool</code>
</li>
<li>
<b>Field added. </b>
<code>bool can_grow</code>
</li>
<li>
<b>Field added. </b>
<code>u64 phys_limit</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head pools</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct dyn_alloc</code>
</li>
<li>
<b>Field removed. </b>
<code>phys_addr_t start</code>
</li>
<li>
<b>Field removed. </b>
<code>phys_addr_t end</code>
</li>
<li>
<b>Field removed. </b>
<code>void *vaddr</code>
</li>
<li>
<b>Field removed. </b>
<code>bool late_alloc</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nareas</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int area_nslabs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_tlb_area *areas</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_tlb_slot *slots</code>
</li>
</ul>
</details>
</li>
</ul>
