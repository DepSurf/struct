# Struct: <code>kfence_metadata</code>

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
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kfence_metadata {
    struct list_head list;
    struct callback_head callback_head;
    raw_spinlock_t lock;
    enum kfence_object_state state;
    long unsigned int addr;
    size_t size;
    struct kmem_cache *cache;
    long unsigned int unprotected_page;
    struct kfence_track alloc_track;
    struct kfence_track free_track;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kfence_metadata {
    struct list_head list;
    struct callback_head callback_head;
    raw_spinlock_t lock;
    enum kfence_object_state state;
    long unsigned int addr;
    size_t size;
    struct kmem_cache *cache;
    long unsigned int unprotected_page;
    struct kfence_track alloc_track;
    struct kfence_track free_track;
    u32 alloc_stack_hash;
    struct obj_cgroup *objcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kfence_metadata {
    struct list_head list;
    struct callback_head callback_head;
    raw_spinlock_t lock;
    enum kfence_object_state state;
    long unsigned int addr;
    size_t size;
    struct kmem_cache *cache;
    long unsigned int unprotected_page;
    struct kfence_track alloc_track;
    struct kfence_track free_track;
    u32 alloc_stack_hash;
    struct obj_cgroup *objcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kfence_metadata {
    struct list_head list;
    struct callback_head callback_head;
    raw_spinlock_t lock;
    enum kfence_object_state state;
    long unsigned int addr;
    size_t size;
    struct kmem_cache *cache;
    long unsigned int unprotected_page;
    struct kfence_track alloc_track;
    struct kfence_track free_track;
    u32 alloc_stack_hash;
    struct obj_cgroup *objcg;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kfence_metadata {
    struct list_head list;
    struct callback_head callback_head;
    raw_spinlock_t lock;
    enum kfence_object_state state;
    long unsigned int addr;
    size_t size;
    struct kmem_cache *cache;
    long unsigned int unprotected_page;
    struct kfence_track alloc_track;
    struct kfence_track free_track;
    u32 alloc_stack_hash;
    struct obj_cgroup *objcg;
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
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 alloc_stack_hash</code>
</li>
<li>
<b>Field added. </b>
<code>struct obj_cgroup *objcg</code>
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
