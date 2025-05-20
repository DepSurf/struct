# Struct: <code>kvm_memslots</code>

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
struct kvm_memslots {
    u64 generation;
    short int id_to_index[512];
    atomic_t lru_slot;
    int used_slots;
    struct kvm_memory_slot memslots[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_memslots {
    u64 generation;
    short int id_to_index[32767];
    atomic_t lru_slot;
    int used_slots;
    struct kvm_memory_slot memslots[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_memslots {
    u64 generation;
    short int id_to_index[32767];
    atomic_t last_used_slot;
    int used_slots;
    struct kvm_memory_slot memslots[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_memslots {
    u64 generation;
    atomic_long_t last_used_slot;
    struct rb_root_cached hva_tree;
    struct rb_root gfn_tree;
    struct hlist_head id_hash[128];
    int node_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_memslots {
    u64 generation;
    atomic_long_t last_used_slot;
    struct rb_root_cached hva_tree;
    struct rb_root gfn_tree;
    struct hlist_head id_hash[128];
    int node_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_memslots {
    u64 generation;
    atomic_long_t last_used_slot;
    struct rb_root_cached hva_tree;
    struct rb_root gfn_tree;
    struct hlist_head id_hash[128];
    int node_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_memslots {
    u64 generation;
    atomic_long_t last_used_slot;
    struct rb_root_cached hva_tree;
    struct rb_root gfn_tree;
    struct hlist_head id_hash[128];
    int node_idx;
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
struct kvm_memslots {
    u64 generation;
    struct kvm_memory_slot memslots[512];
    short int id_to_index[512];
    atomic_t lru_slot;
    int used_slots;
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
struct kvm_memslots {
    u64 generation;
    struct kvm_memory_slot memslots[512];
    short int id_to_index[512];
    atomic_t lru_slot;
    int used_slots;
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>short int id_to_index[512]</code> ➡️ <code>short int id_to_index[32767]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t last_used_slot</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t lru_slot</code>
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
<code>struct rb_root_cached hva_tree</code>
</li>
<li>
<b>Field added. </b>
<code>struct rb_root gfn_tree</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_head id_hash[128]</code>
</li>
<li>
<b>Field added. </b>
<code>int node_idx</code>
</li>
<li>
<b>Field removed. </b>
<code>short int id_to_index[32767]</code>
</li>
<li>
<b>Field removed. </b>
<code>int used_slots</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kvm_memory_slot memslots[0]</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_t last_used_slot</code> ➡️ <code>atomic_long_t last_used_slot</code>
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
<b>Arch</b>
<ul>
</ul>
