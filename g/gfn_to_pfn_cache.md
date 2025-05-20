# Struct: <code>gfn_to_pfn_cache</code>

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
struct gfn_to_pfn_cache {
    u64 generation;
    gfn_t gfn;
    kvm_pfn_t pfn;
    bool dirty;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct gfn_to_pfn_cache {
    u64 generation;
    gfn_t gfn;
    kvm_pfn_t pfn;
    bool dirty;
};
```
</details>
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct gfn_to_pfn_cache {
    u64 generation;
    gpa_t gpa;
    long unsigned int uhva;
    struct kvm_memory_slot *memslot;
    struct kvm_vcpu *vcpu;
    struct list_head list;
    rwlock_t lock;
    struct mutex refresh_lock;
    void *khva;
    kvm_pfn_t pfn;
    enum pfn_cache_usage usage;
    bool active;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct gfn_to_pfn_cache {
    u64 generation;
    gpa_t gpa;
    long unsigned int uhva;
    struct kvm_memory_slot *memslot;
    struct kvm *kvm;
    struct kvm_vcpu *vcpu;
    struct list_head list;
    rwlock_t lock;
    struct mutex refresh_lock;
    void *khva;
    kvm_pfn_t pfn;
    enum pfn_cache_usage usage;
    bool active;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct gfn_to_pfn_cache {
    u64 generation;
    gpa_t gpa;
    long unsigned int uhva;
    struct kvm_memory_slot *memslot;
    struct kvm *kvm;
    struct kvm_vcpu *vcpu;
    struct list_head list;
    rwlock_t lock;
    struct mutex refresh_lock;
    void *khva;
    kvm_pfn_t pfn;
    enum pfn_cache_usage usage;
    bool active;
    bool valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct gfn_to_pfn_cache {
    u64 generation;
    gpa_t gpa;
    long unsigned int uhva;
    struct kvm_memory_slot *memslot;
    struct kvm *kvm;
    struct kvm_vcpu *vcpu;
    struct list_head list;
    rwlock_t lock;
    struct mutex refresh_lock;
    void *khva;
    kvm_pfn_t pfn;
    enum pfn_cache_usage usage;
    bool active;
    bool valid;
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
struct gfn_to_pfn_cache {
    u64 generation;
    gfn_t gfn;
    kvm_pfn_t pfn;
    bool dirty;
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kvm *kvm</code>
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
