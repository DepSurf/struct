# Struct: <code>kiocb</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    enum rw_hint ki_hint;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    enum rw_hint ki_hint;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
    struct wait_page_queue *ki_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
    struct wait_page_queue *ki_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
    struct wait_page_queue *ki_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int);
    void *private;
    int ki_flags;
    u16 ki_ioprio;
    struct wait_page_queue *ki_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int);
    void *private;
    int ki_flags;
    u16 ki_ioprio;
    struct wait_page_queue *ki_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int);
    void *private;
    int ki_flags;
    u16 ki_ioprio;
    struct wait_page_queue *ki_waitq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int);
    void *private;
    int ki_flags;
    u16 ki_ioprio;
    struct wait_page_queue *ki_waitq;
    ssize_t (*dio_complete)(void *);
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
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
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
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kiocb {
    struct file *ki_filp;
    loff_t ki_pos;
    void (*ki_complete)(struct kiocb *, long int, long int);
    void *private;
    int ki_flags;
    u16 ki_hint;
    u16 ki_ioprio;
    unsigned int ki_cookie;
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
<b>Field added. </b>
<code>enum rw_hint ki_hint</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 ki_ioprio</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum rw_hint ki_hint</code> ➡️ <code>u16 ki_hint</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int ki_cookie</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct wait_page_queue *ki_waitq</code>
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
<code>u16 ki_hint</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int ki_cookie</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*ki_complete)(struct kiocb *, long int, long int)</code> ➡️ <code>void (*ki_complete)(struct kiocb *, long int)</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>ssize_t (*dio_complete)(void *)</code>
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
