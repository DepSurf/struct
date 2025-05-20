# Struct: <code>fuse_conn_dax</code>

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
struct fuse_conn_dax {
    struct dax_device *dev;
    spinlock_t lock;
    long unsigned int nr_busy_ranges;
    struct list_head busy_ranges;
    struct delayed_work free_work;
    wait_queue_head_t range_waitq;
    long int nr_free_ranges;
    struct list_head free_ranges;
    long unsigned int nr_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fuse_conn_dax {
    struct dax_device *dev;
    spinlock_t lock;
    long unsigned int nr_busy_ranges;
    struct list_head busy_ranges;
    struct delayed_work free_work;
    wait_queue_head_t range_waitq;
    long int nr_free_ranges;
    struct list_head free_ranges;
    long unsigned int nr_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fuse_conn_dax {
    struct dax_device *dev;
    spinlock_t lock;
    long unsigned int nr_busy_ranges;
    struct list_head busy_ranges;
    struct delayed_work free_work;
    wait_queue_head_t range_waitq;
    long int nr_free_ranges;
    struct list_head free_ranges;
    long unsigned int nr_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fuse_conn_dax {
    struct dax_device *dev;
    spinlock_t lock;
    long unsigned int nr_busy_ranges;
    struct list_head busy_ranges;
    struct delayed_work free_work;
    wait_queue_head_t range_waitq;
    long int nr_free_ranges;
    struct list_head free_ranges;
    long unsigned int nr_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fuse_conn_dax {
    struct dax_device *dev;
    spinlock_t lock;
    long unsigned int nr_busy_ranges;
    struct list_head busy_ranges;
    struct delayed_work free_work;
    wait_queue_head_t range_waitq;
    long int nr_free_ranges;
    struct list_head free_ranges;
    long unsigned int nr_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fuse_conn_dax {
    struct dax_device *dev;
    spinlock_t lock;
    long unsigned int nr_busy_ranges;
    struct list_head busy_ranges;
    struct delayed_work free_work;
    wait_queue_head_t range_waitq;
    long int nr_free_ranges;
    struct list_head free_ranges;
    long unsigned int nr_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fuse_conn_dax {
    struct dax_device *dev;
    spinlock_t lock;
    long unsigned int nr_busy_ranges;
    struct list_head busy_ranges;
    struct delayed_work free_work;
    wait_queue_head_t range_waitq;
    long int nr_free_ranges;
    struct list_head free_ranges;
    long unsigned int nr_ranges;
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
