# Struct: <code>bpf_dtab</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    long unsigned int *flush_needed;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    long unsigned int *flush_needed;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    long unsigned int *flush_needed;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
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
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
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
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_dtab {
    struct bpf_map map;
    struct bpf_dtab_netdev **netdev_map;
    struct list_head *flush_list;
    struct list_head list;
    struct hlist_head *dev_index_head;
    spinlock_t index_lock;
    unsigned int items;
    u32 n_buckets;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<code>struct list_head *flush_list</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int *flush_needed</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_head *dev_index_head</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t index_lock</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int items</code>
</li>
<li>
<b>Field added. </b>
<code>u32 n_buckets</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head *flush_list</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
