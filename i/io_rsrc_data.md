# Struct: <code>io_rsrc_data</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_rsrc_data {
    struct io_ring_ctx *ctx;
    u64 *tags;
    rsrc_put_fn *do_put;
    atomic_t refs;
    struct completion done;
    bool quiesce;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_rsrc_data {
    struct io_ring_ctx *ctx;
    u64 **tags;
    unsigned int nr;
    rsrc_put_fn *do_put;
    atomic_t refs;
    struct completion done;
    bool quiesce;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_rsrc_data {
    struct io_ring_ctx *ctx;
    u64 **tags;
    unsigned int nr;
    rsrc_put_fn *do_put;
    atomic_t refs;
    struct completion done;
    bool quiesce;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_rsrc_data {
    struct io_ring_ctx *ctx;
    u64 **tags;
    unsigned int nr;
    rsrc_put_fn *do_put;
    atomic_t refs;
    struct completion done;
    bool quiesce;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_rsrc_data {
    struct io_ring_ctx *ctx;
    u64 **tags;
    unsigned int nr;
    u16 rsrc_type;
    bool quiesce;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_rsrc_data {
    struct io_ring_ctx *ctx;
    u64 **tags;
    unsigned int nr;
    u16 rsrc_type;
    bool quiesce;
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
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int nr</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 *tags</code> ➡️ <code>u64 **tags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 rsrc_type</code>
</li>
<li>
<b>Field removed. </b>
<code>rsrc_put_fn *do_put</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t refs</code>
</li>
<li>
<b>Field removed. </b>
<code>struct completion done</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
