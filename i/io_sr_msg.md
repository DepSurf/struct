# Struct: <code>io_sr_msg</code>

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
struct io_sr_msg {
    struct file *file;
    struct user_msghdr *msg;
    void *buf;
    int msg_flags;
    int bgid;
    size_t len;
    struct io_buffer *kbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct io_sr_msg {
    struct file *file;
    struct user_msghdr *umsg;
    void *buf;
    int msg_flags;
    int bgid;
    size_t len;
    struct io_buffer *kbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct io_sr_msg {
    struct file *file;
    struct compat_msghdr *umsg_compat;
    struct user_msghdr *umsg;
    void *buf;
    int msg_flags;
    int bgid;
    size_t len;
    struct io_buffer *kbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct io_sr_msg {
    struct file *file;
    struct compat_msghdr *umsg_compat;
    struct user_msghdr *umsg;
    void *buf;
    int msg_flags;
    int bgid;
    size_t len;
    struct io_buffer *kbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct io_sr_msg {
    struct file *file;
    struct compat_msghdr *umsg_compat;
    struct user_msghdr *umsg;
    void *buf;
    int msg_flags;
    size_t len;
    size_t done_io;
    unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_sr_msg {
    struct file *file;
    struct compat_msghdr *umsg_compat;
    struct user_msghdr *umsg;
    void *buf;
    unsigned int len;
    unsigned int done_io;
    unsigned int msg_flags;
    u16 flags;
    u16 addr_len;
    u16 buf_group;
    void *addr;
    struct io_kiocb *notif;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_sr_msg {
    struct file *file;
    struct compat_msghdr *umsg_compat;
    struct user_msghdr *umsg;
    void *buf;
    unsigned int len;
    unsigned int done_io;
    unsigned int msg_flags;
    u16 flags;
    u16 addr_len;
    u16 buf_group;
    void *addr;
    void *msg_control;
    struct io_kiocb *notif;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_sr_msg {
    struct file *file;
    struct compat_msghdr *umsg_compat;
    struct user_msghdr *umsg;
    void *buf;
    unsigned int len;
    unsigned int done_io;
    unsigned int msg_flags;
    unsigned int nr_multishot_loops;
    u16 flags;
    u16 addr_len;
    u16 buf_group;
    void *addr;
    void *msg_control;
    struct io_kiocb *notif;
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
<code>struct user_msghdr *umsg</code>
</li>
<li>
<b>Field removed. </b>
<code>struct user_msghdr *msg</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct compat_msghdr *umsg_compat</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t done_io</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int flags</code>
</li>
<li>
<b>Field removed. </b>
<code>int bgid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct io_buffer *kbuf</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 addr_len</code>
</li>
<li>
<b>Field added. </b>
<code>u16 buf_group</code>
</li>
<li>
<b>Field added. </b>
<code>void *addr</code>
</li>
<li>
<b>Field added. </b>
<code>struct io_kiocb *notif</code>
</li>
<li>
<b>Field type changed. </b>
<code>int msg_flags</code> ➡️ <code>unsigned int msg_flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t len</code> ➡️ <code>unsigned int len</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t done_io</code> ➡️ <code>unsigned int done_io</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int flags</code> ➡️ <code>u16 flags</code>
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
<code>void *msg_control</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int nr_multishot_loops</code>
</li>
</ul>
</details>
</li>
</ul>
