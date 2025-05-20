# Struct: <code>bpf_htab</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct hlist_head *buckets;
    raw_spinlock_t lock;
    u32 count;
    u32 n_buckets;
    u32 elem_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    void *extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    void *extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
    struct lock_class_key lockdep_key;
    int * map_locked[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
    struct lock_class_key lockdep_key;
    int * map_locked[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
    struct lock_class_key lockdep_key;
    int * map_locked[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
    struct lock_class_key lockdep_key;
    int * map_locked[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bpf_mem_alloc ma;
    struct bpf_mem_alloc pcpu_ma;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    struct percpu_counter pcount;
    atomic_t count;
    bool use_percpu_counter;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
    struct lock_class_key lockdep_key;
    int * map_locked[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bpf_mem_alloc ma;
    struct bpf_mem_alloc pcpu_ma;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    struct percpu_counter pcount;
    atomic_t count;
    bool use_percpu_counter;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
    struct lock_class_key lockdep_key;
    int * map_locked[8];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bpf_mem_alloc ma;
    struct bpf_mem_alloc pcpu_ma;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    struct percpu_counter pcount;
    atomic_t count;
    bool use_percpu_counter;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
    struct lock_class_key lockdep_key;
    int * map_locked[8];
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
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
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
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_htab {
    struct bpf_map map;
    struct bucket *buckets;
    void *elems;
    struct pcpu_freelist freelist;
    struct bpf_lru lru;
    struct htab_elem **extra_elems;
    atomic_t count;
    u32 n_buckets;
    u32 elem_size;
    u32 hashrnd;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *elems</code>
</li>
<li>
<b>Field added. </b>
<code>struct pcpu_freelist freelist</code>
</li>
<li>
<b>Field added. </b>
<code>void *extra_elems</code>
</li>
<li>
<b>Field removed. </b>
<code>raw_spinlock_t lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct hlist_head *buckets</code> ➡️ <code>struct bucket *buckets</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 count</code> ➡️ <code>atomic_t count</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bpf_lru lru</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void *extra_elems</code> ➡️ <code>struct htab_elem **extra_elems</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 hashrnd</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct lock_class_key lockdep_key</code>
</li>
<li>
<b>Field added. </b>
<code>int * map_locked[8]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bpf_mem_alloc ma</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_mem_alloc pcpu_ma</code>
</li>
<li>
<b>Field added. </b>
<code>struct percpu_counter pcount</code>
</li>
<li>
<b>Field added. </b>
<code>bool use_percpu_counter</code>
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
