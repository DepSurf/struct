# Struct: <code>memcg_cache_params</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct memcg_cache_params {
    bool is_root_cache;
    struct list_head list;
    struct memcg_cache_array *memcg_caches;
    struct mem_cgroup *memcg;
    struct kmem_cache *root_cache;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct memcg_cache_params {
    bool is_root_cache;
    struct list_head list;
    struct memcg_cache_array *memcg_caches;
    struct mem_cgroup *memcg;
    struct kmem_cache *root_cache;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct memcg_cache_params {
    bool is_root_cache;
    struct list_head list;
    struct memcg_cache_array *memcg_caches;
    struct mem_cgroup *memcg;
    struct kmem_cache *root_cache;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    void (*deact_fn)(struct kmem_cache *);
    struct callback_head deact_rcu_head;
    struct work_struct deact_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    void (*deact_fn)(struct kmem_cache *);
    struct callback_head deact_rcu_head;
    struct work_struct deact_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    void (*deact_fn)(struct kmem_cache *);
    struct callback_head deact_rcu_head;
    struct work_struct deact_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    void (*deact_fn)(struct kmem_cache *);
    struct callback_head deact_rcu_head;
    struct work_struct deact_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
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
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
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
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct memcg_cache_params {
    struct kmem_cache *root_cache;
    struct memcg_cache_array *memcg_caches;
    struct list_head __root_caches_node;
    struct list_head children;
    bool dying;
    struct mem_cgroup *memcg;
    struct list_head children_node;
    struct list_head kmem_caches_node;
    struct percpu_ref refcnt;
    void (*work_fn)(struct kmem_cache *);
    struct callback_head callback_head;
    struct work_struct work;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head __root_caches_node</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head children</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head children_node</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head kmem_caches_node</code>
</li>
<li>
<b>Field added. </b>
<code>void (*deact_fn)(struct kmem_cache *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head deact_rcu_head</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct deact_work</code>
</li>
<li>
<b>Field removed. </b>
<code>bool is_root_cache</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool dying</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct percpu_ref refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>void (*work_fn)(struct kmem_cache *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head callback_head</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct work</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*deact_fn)(struct kmem_cache *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head deact_rcu_head</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct deact_work</code>
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
