# Struct: <code>tracing_map</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[5];
    unsigned int n_fields;
    int key_idx[2];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[5];
    unsigned int n_fields;
    int key_idx[2];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[5];
    unsigned int n_fields;
    int key_idx[2];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
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
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
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
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tracing_map {
    unsigned int key_size;
    unsigned int map_bits;
    unsigned int map_size;
    unsigned int max_elts;
    atomic_t next_elt;
    struct tracing_map_array *elts;
    struct tracing_map_array *map;
    const struct tracing_map_ops *ops;
    void *private_data;
    struct tracing_map_field fields[6];
    unsigned int n_fields;
    int key_idx[3];
    unsigned int n_keys;
    struct tracing_map_sort_key sort_key;
    unsigned int n_vars;
    atomic64_t hits;
    atomic64_t drops;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct tracing_map_field fields[5]</code> ➡️ <code>struct tracing_map_field fields[6]</code>
</li>
<li>
<b>Field type changed. </b>
<code>int key_idx[2]</code> ➡️ <code>int key_idx[3]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int n_vars</code>
</li>
</ul>
</details>
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
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
