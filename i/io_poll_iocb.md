# Struct: <code>io_poll_iocb</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    u64 addr;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
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
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct io_poll_iocb {
    struct file *file;
    struct wait_queue_head *head;
    __poll_t events;
    bool done;
    bool canceled;
    struct wait_queue_entry wait;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 addr</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 addr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool done</code>
</li>
<li>
<b>Field removed. </b>
<code>bool canceled</code>
</li>
</ul>
</details>
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
