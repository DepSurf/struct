# Struct: <code>sidtab</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct sidtab {
    struct sidtab_node **htable;
    unsigned int nel;
    unsigned int next_sid;
    unsigned char shutdown;
    struct sidtab_node * cache[3];
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct sidtab {
    struct sidtab_node **htable;
    unsigned int nel;
    unsigned int next_sid;
    unsigned char shutdown;
    struct sidtab_node * cache[3];
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct sidtab {
    struct sidtab_node **htable;
    unsigned int nel;
    unsigned int next_sid;
    unsigned char shutdown;
    struct sidtab_node * cache[3];
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct sidtab {
    struct sidtab_node **htable;
    unsigned int nel;
    unsigned int next_sid;
    unsigned char shutdown;
    struct sidtab_node * cache[3];
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct sidtab {
    struct sidtab_node **htable;
    unsigned int nel;
    unsigned int next_sid;
    unsigned char shutdown;
    struct sidtab_node * cache[3];
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sidtab {
    struct sidtab_node **htable;
    unsigned int nel;
    unsigned int next_sid;
    unsigned char shutdown;
    struct sidtab_node * cache[3];
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    atomic_t count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    atomic_t rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    atomic_t count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    atomic_t rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    bool frozen;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    bool frozen;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    bool frozen;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    bool frozen;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    bool frozen;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    bool frozen;
    spinlock_t lock;
    u32 cache_free_slots;
    struct list_head cache_lru_list;
    spinlock_t cache_lock;
    struct sidtab_isid_entry isids[27];
    struct hlist_head context_to_sid[512];
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
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[3];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
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
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sidtab {
    union sidtab_entry_inner roots[4];
    u32 count;
    struct sidtab_convert_params *convert;
    spinlock_t lock;
    u32 rcache[3];
    struct sidtab_isid_entry isids[27];
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
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
<code>union sidtab_entry_inner roots[4]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t count</code>
</li>
<li>
<b>Field added. </b>
<code>struct sidtab_convert_params *convert</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t rcache[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct sidtab_isid_entry isids[27]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sidtab_node **htable</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nel</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int next_sid</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char shutdown</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sidtab_node * cache[3]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t count</code> ➡️ <code>u32 count</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t rcache[3]</code> ➡️ <code>u32 rcache[3]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 cache_free_slots</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head cache_lru_list</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t cache_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_head context_to_sid[512]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 rcache[3]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool frozen</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>union sidtab_entry_inner roots[4]</code> ➡️ <code>union sidtab_entry_inner roots[3]</code>
</li>
</ul>
</details>
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
