# Struct: <code>fuse_args</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fuse_args {
    struct (anon) in;
    struct (anon) out;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_mount *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_mount *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool user_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_mount *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool user_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_mount *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool user_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_mount *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    uint8_t in_numargs;
    uint8_t out_numargs;
    uint8_t ext_idx;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool user_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    bool is_ext;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_mount *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    uint8_t in_numargs;
    uint8_t out_numargs;
    uint8_t ext_idx;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool user_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    bool may_block;
    bool is_ext;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_mount *, struct fuse_args *, int);
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
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
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
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fuse_args {
    uint64_t nodeid;
    uint32_t opcode;
    short unsigned int in_numargs;
    short unsigned int out_numargs;
    bool force;
    bool noreply;
    bool nocreds;
    bool in_pages;
    bool out_pages;
    bool out_argvar;
    bool page_zeroing;
    bool page_replace;
    struct fuse_in_arg in_args[3];
    struct fuse_arg out_args[2];
    void (*end)(struct fuse_conn *, struct fuse_args *, int);
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
No changes between <code>4.13</code> and <code>4.15</code> ✅
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>uint64_t nodeid</code>
</li>
<li>
<b>Field added. </b>
<code>uint32_t opcode</code>
</li>
<li>
<b>Field added. </b>
<code>short unsigned int in_numargs</code>
</li>
<li>
<b>Field added. </b>
<code>short unsigned int out_numargs</code>
</li>
<li>
<b>Field added. </b>
<code>bool force</code>
</li>
<li>
<b>Field added. </b>
<code>bool noreply</code>
</li>
<li>
<b>Field added. </b>
<code>bool nocreds</code>
</li>
<li>
<b>Field added. </b>
<code>bool in_pages</code>
</li>
<li>
<b>Field added. </b>
<code>bool out_pages</code>
</li>
<li>
<b>Field added. </b>
<code>bool out_argvar</code>
</li>
<li>
<b>Field added. </b>
<code>bool page_zeroing</code>
</li>
<li>
<b>Field added. </b>
<code>bool page_replace</code>
</li>
<li>
<b>Field added. </b>
<code>struct fuse_in_arg in_args[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct fuse_arg out_args[2]</code>
</li>
<li>
<b>Field added. </b>
<code>void (*end)(struct fuse_conn *, struct fuse_args *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) in</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) out</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool may_block</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*end)(struct fuse_conn *, struct fuse_args *, int)</code> ➡️ <code>void (*end)(struct fuse_mount *, struct fuse_args *, int)</code>
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
<code>bool user_pages</code>
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
<code>uint8_t ext_idx</code>
</li>
<li>
<b>Field added. </b>
<code>bool is_ext</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int in_numargs</code> ➡️ <code>uint8_t in_numargs</code>
</li>
<li>
<b>Field type changed. </b>
<code>short unsigned int out_numargs</code> ➡️ <code>uint8_t out_numargs</code>
</li>
</ul>
</details>
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
