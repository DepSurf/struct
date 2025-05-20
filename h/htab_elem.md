# Struct: <code>htab_elem</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_node hash_node;
    struct callback_head rcu;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_node hash_node;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    enum extra_elem_state state;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_node hash_node;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    enum extra_elem_state state;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    void *ptr_to_pptr;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    void *ptr_to_pptr;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct pcpu_freelist_node fnode;
    struct htab_elem *batch_flink;
    void *ptr_to_pptr;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
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
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
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
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct htab_elem {
    struct hlist_nulls_node hash_node;
    void *padding;
    struct bpf_htab *htab;
    struct pcpu_freelist_node fnode;
    struct callback_head rcu;
    struct bpf_lru_node lru_node;
    u32 hash;
    char key[0];
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
<code>struct bpf_htab *htab</code>
</li>
<li>
<b>Field added. </b>
<code>struct pcpu_freelist_node fnode</code>
</li>
<li>
<b>Field added. </b>
<code>enum extra_elem_state state</code>
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
<code>struct bpf_lru_node lru_node</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *padding</code>
</li>
<li>
<b>Field removed. </b>
<code>enum extra_elem_state state</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct hlist_node hash_node</code> ➡️ <code>struct hlist_nulls_node hash_node</code>
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct htab_elem *batch_flink</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *ptr_to_pptr</code>
</li>
<li>
<b>Field removed. </b>
<code>struct bpf_htab *htab</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head rcu</code>
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
