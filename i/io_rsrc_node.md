# Struct: <code>io_rsrc_node</code>

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
struct io_rsrc_node {
    struct percpu_ref refs;
    struct list_head node;
    struct list_head rsrc_list;
    struct io_rsrc_data *rsrc_data;
    struct llist_node llist;
    bool done;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_rsrc_node {
    struct percpu_ref refs;
    struct list_head node;
    struct list_head rsrc_list;
    struct io_rsrc_data *rsrc_data;
    struct llist_node llist;
    bool done;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_rsrc_node {
    struct percpu_ref refs;
    struct list_head node;
    struct list_head rsrc_list;
    struct io_rsrc_data *rsrc_data;
    struct llist_node llist;
    bool done;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_rsrc_node {
    struct percpu_ref refs;
    struct list_head node;
    struct list_head rsrc_list;
    struct io_rsrc_data *rsrc_data;
    struct llist_node llist;
    bool done;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_rsrc_node {
    struct io_cache_entry cache;
    struct io_ring_ctx *ctx;
    int refs;
    bool empty;
    u16 type;
    struct list_head node;
    struct io_rsrc_put item;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_rsrc_node {
    struct io_cache_entry cache;
    struct io_ring_ctx *ctx;
    int refs;
    bool empty;
    u16 type;
    struct list_head node;
    struct io_rsrc_put item;
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
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
<code>struct io_cache_entry cache</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_ring_ctx *ctx</code>
</li>
<li>
<b>Field added. </b>
<code>bool empty</code>
</li>
<li>
<b>Field added. </b>
<code>u16 type</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_rsrc_put item</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head rsrc_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_rsrc_data *rsrc_data</code>
</li>
<li>
<b>Field removed. </b>
<code>struct llist_node llist</code>
</li>
<li>
<b>Field removed. </b>
<code>bool done</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct percpu_ref refs</code> ➡️ <code>int refs</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
