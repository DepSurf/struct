# Struct: <code>slab</code>

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
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct slab {
    long unsigned int __page_flags;
    struct list_head slab_list;
    struct callback_head callback_head;
    struct slab *next;
    int slabs;
    struct kmem_cache *slab_cache;
    void *freelist;
    long unsigned int counters;
    unsigned int inuse;
    unsigned int objects;
    unsigned int frozen;
    unsigned int __unused;
    atomic_t __page_refcount;
    long unsigned int memcg_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct slab {
    long unsigned int __page_flags;
    struct kmem_cache *slab_cache;
    struct list_head slab_list;
    struct slab *next;
    int slabs;
    void *freelist;
    long unsigned int counters;
    unsigned int inuse;
    unsigned int objects;
    unsigned int frozen;
    struct callback_head callback_head;
    unsigned int __unused;
    atomic_t __page_refcount;
    long unsigned int memcg_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct slab {
    long unsigned int __page_flags;
    struct kmem_cache *slab_cache;
    struct list_head slab_list;
    struct slab *next;
    int slabs;
    void *freelist;
    long unsigned int counters;
    unsigned int inuse;
    unsigned int objects;
    unsigned int frozen;
    freelist_aba_t freelist_counter;
    struct callback_head callback_head;
    unsigned int __unused;
    atomic_t __page_refcount;
    long unsigned int memcg_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct slab {
    long unsigned int __page_flags;
    struct kmem_cache *slab_cache;
    struct list_head slab_list;
    struct slab *next;
    int slabs;
    void *freelist;
    long unsigned int counters;
    unsigned int inuse;
    unsigned int objects;
    unsigned int frozen;
    freelist_aba_t freelist_counter;
    struct callback_head callback_head;
    unsigned int __unused;
    atomic_t __page_refcount;
    long unsigned int memcg_data;
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
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>freelist_aba_t freelist_counter</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
