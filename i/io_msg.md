# Struct: <code>io_msg</code>

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
struct io_msg {
    struct file *file;
    u64 user_data;
    u32 len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct io_msg {
    struct file *file;
    struct file *src_file;
    struct callback_head tw;
    u64 user_data;
    u32 len;
    u32 cmd;
    u32 src_fd;
    u32 dst_fd;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct io_msg {
    struct file *file;
    struct file *src_file;
    struct callback_head tw;
    u64 user_data;
    u32 len;
    u32 cmd;
    u32 src_fd;
    u32 dst_fd;
    u32 cqe_flags;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct io_msg {
    struct file *file;
    struct file *src_file;
    struct callback_head tw;
    u64 user_data;
    u32 len;
    u32 cmd;
    u32 src_fd;
    u32 dst_fd;
    u32 cqe_flags;
    u32 flags;
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
<code>struct file *src_file</code>
</li>
<li>
<b>Field added. </b>
<code>struct callback_head tw</code>
</li>
<li>
<b>Field added. </b>
<code>u32 cmd</code>
</li>
<li>
<b>Field added. </b>
<code>u32 src_fd</code>
</li>
<li>
<b>Field added. </b>
<code>u32 dst_fd</code>
</li>
<li>
<b>Field added. </b>
<code>u32 flags</code>
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
<code>u32 cqe_flags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
