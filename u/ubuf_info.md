# Struct: <code>ubuf_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    void *ctx;
    long unsigned int desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    void *ctx;
    long unsigned int desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    void *ctx;
    long unsigned int desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    void *ctx;
    long unsigned int desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct sk_buff *, struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    u8 flags;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct sk_buff *, struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    u8 flags;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct sk_buff *, struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    u8 flags;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct sk_buff *, struct ubuf_info *, bool);
    refcount_t refcnt;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct sk_buff *, struct ubuf_info *, bool);
    refcount_t refcnt;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct sk_buff *, struct ubuf_info *, bool);
    refcount_t refcnt;
    u8 flags;
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
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
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
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ubuf_info {
    void (*callback)(struct ubuf_info *, bool);
    long unsigned int desc;
    void *ctx;
    u32 id;
    u16 len;
    u16 zerocopy;
    u32 bytelen;
    refcount_t refcnt;
    struct mmpin mmp;
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 id</code>
</li>
<li>
<b>Field added. </b>
<code>u16 len</code>
</li>
<li>
<b>Field added. </b>
<code>u16 zerocopy</code>
</li>
<li>
<b>Field added. </b>
<code>u32 bytelen</code>
</li>
<li>
<b>Field added. </b>
<code>refcount_t refcnt</code>
</li>
<li>
<b>Field added. </b>
<code>struct mmpin mmp</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 flags</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*callback)(struct ubuf_info *, bool)</code> ➡️ <code>void (*callback)(struct sk_buff *, struct ubuf_info *, bool)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int desc</code>
</li>
<li>
<b>Field removed. </b>
<code>void *ctx</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 id</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 len</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 zerocopy</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 bytelen</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mmpin mmp</code>
</li>
</ul>
</details>
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
