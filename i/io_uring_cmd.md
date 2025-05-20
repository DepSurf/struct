# Struct: <code>io_uring_cmd</code>

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
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_uring_cmd {
    struct file *file;
    const void *cmd;
    void (*task_work_cb)(struct io_uring_cmd *);
    u32 cmd_op;
    u32 pad;
    u8 pdu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_uring_cmd {
    struct file *file;
    const void *cmd;
    void (*task_work_cb)(struct io_uring_cmd *);
    void *cookie;
    u32 cmd_op;
    u32 flags;
    u8 pdu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_uring_cmd {
    struct file *file;
    const struct io_uring_sqe *sqe;
    void (*task_work_cb)(struct io_uring_cmd *, unsigned int);
    void *cookie;
    u32 cmd_op;
    u32 flags;
    u8 pdu[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_uring_cmd {
    struct file *file;
    const struct io_uring_sqe *sqe;
    void (*task_work_cb)(struct io_uring_cmd *, unsigned int);
    u32 cmd_op;
    u32 flags;
    u8 pdu[32];
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
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *cookie</code>
</li>
<li>
<b>Field added. </b>
<code>u32 flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 pad</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct io_uring_sqe *sqe</code>
</li>
<li>
<b>Field removed. </b>
<code>const void *cmd</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*task_work_cb)(struct io_uring_cmd *)</code> ➡️ <code>void (*task_work_cb)(struct io_uring_cmd *, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void *cookie</code>
</li>
</ul>
</details>
</li>
</ul>
