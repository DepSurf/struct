# Struct: <code>rhashtable_params</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rhashtable_params {
    size_t nelem_hint;
    size_t key_len;
    size_t key_offset;
    size_t head_offset;
    unsigned int insecure_max_entries;
    unsigned int max_size;
    unsigned int min_size;
    u32 nulls_base;
    bool insecure_elasticity;
    bool automatic_shrinking;
    size_t locks_mul;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rhashtable_params {
    size_t nelem_hint;
    size_t key_len;
    size_t key_offset;
    size_t head_offset;
    unsigned int insecure_max_entries;
    unsigned int max_size;
    unsigned int min_size;
    u32 nulls_base;
    bool insecure_elasticity;
    bool automatic_shrinking;
    size_t locks_mul;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rhashtable_params {
    size_t nelem_hint;
    size_t key_len;
    size_t key_offset;
    size_t head_offset;
    unsigned int insecure_max_entries;
    unsigned int max_size;
    unsigned int min_size;
    u32 nulls_base;
    bool insecure_elasticity;
    bool automatic_shrinking;
    size_t locks_mul;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    u8 locks_mul;
    u32 nulls_base;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    u8 locks_mul;
    u32 nulls_base;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    u8 locks_mul;
    u32 nulls_base;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    u8 locks_mul;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
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
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
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
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rhashtable_params {
    u16 nelem_hint;
    u16 key_len;
    u16 key_offset;
    u16 head_offset;
    unsigned int max_size;
    u16 min_size;
    bool automatic_shrinking;
    rht_hashfn_t hashfn;
    rht_obj_hashfn_t obj_hashfn;
    rht_obj_cmpfn_t obj_cmpfn;
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
<b>Field removed. </b>
<code>unsigned int insecure_max_entries</code>
</li>
<li>
<b>Field removed. </b>
<code>bool insecure_elasticity</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t nelem_hint</code> ➡️ <code>u16 nelem_hint</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t key_len</code> ➡️ <code>u16 key_len</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t key_offset</code> ➡️ <code>u16 key_offset</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t head_offset</code> ➡️ <code>u16 head_offset</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int min_size</code> ➡️ <code>u16 min_size</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t locks_mul</code> ➡️ <code>u8 locks_mul</code>
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
<b>Field removed. </b>
<code>u32 nulls_base</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u8 locks_mul</code>
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
