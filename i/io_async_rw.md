# Struct: <code>io_async_rw</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct io_async_rw {
    struct iovec fast_iov[8];
    struct iovec *iov;
    ssize_t nr_segs;
    ssize_t size;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_async_rw {
    struct iovec fast_iov[8];
    const struct iovec *free_iovec;
    struct iov_iter iter;
    size_t bytes_done;
    struct wait_page_queue wpq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_async_rw {
    struct iovec fast_iov[8];
    const struct iovec *free_iovec;
    struct iov_iter iter;
    size_t bytes_done;
    struct wait_page_queue wpq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_async_rw {
    struct iovec fast_iov[8];
    const struct iovec *free_iovec;
    struct iov_iter iter;
    struct iov_iter_state iter_state;
    size_t bytes_done;
    struct wait_page_queue wpq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_async_rw {
    struct io_rw_state s;
    const struct iovec *free_iovec;
    size_t bytes_done;
    struct wait_page_queue wpq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_async_rw {
    struct io_rw_state s;
    const struct iovec *free_iovec;
    size_t bytes_done;
    struct wait_page_queue wpq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_async_rw {
    struct io_rw_state s;
    const struct iovec *free_iovec;
    size_t bytes_done;
    struct wait_page_queue wpq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_async_rw {
    struct io_rw_state s;
    const struct iovec *free_iovec;
    size_t bytes_done;
    struct wait_page_queue wpq;
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct iovec *free_iovec</code>
</li>
<li>
<b>Field added. </b>
<code>struct iov_iter iter</code>
</li>
<li>
<b>Field added. </b>
<code>size_t bytes_done</code>
</li>
<li>
<b>Field added. </b>
<code>struct wait_page_queue wpq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iovec *iov</code>
</li>
<li>
<b>Field removed. </b>
<code>ssize_t nr_segs</code>
</li>
<li>
<b>Field removed. </b>
<code>ssize_t size</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iov_iter_state iter_state</code>
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
<code>struct io_rw_state s</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iovec fast_iov[8]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iov_iter iter</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iov_iter_state iter_state</code>
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
