# Struct: <code>fuse_req</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    atomic_t count;
    u64 intr_unique;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    atomic_t count;
    u64 intr_unique;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    atomic_t count;
    u64 intr_unique;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    refcount_t count;
    u64 intr_unique;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    refcount_t count;
    u64 intr_unique;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    refcount_t count;
    u64 intr_unique;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    refcount_t count;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    refcount_t count;
    long unsigned int flags;
    struct fuse_in in;
    struct fuse_out out;
    wait_queue_head_t waitq;
    union (anon) misc;
    struct page **pages;
    struct fuse_page_desc *page_descs;
    unsigned int max_pages;
    struct page * inline_pages[1];
    struct fuse_page_desc inline_page_descs[1];
    unsigned int num_pages;
    struct fuse_file *ff;
    struct inode *inode;
    struct fuse_io_priv *io;
    struct list_head writepages_entry;
    void (*end)(struct fuse_conn *, struct fuse_req *);
    struct file *stolen_file;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
    struct fuse_mount *fm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
    struct fuse_mount *fm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
    struct fuse_mount *fm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
    struct fuse_mount *fm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
    struct fuse_mount *fm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
    struct fuse_mount *fm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
    struct fuse_mount *fm;
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
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
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
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fuse_req {
    struct list_head list;
    struct list_head intr_entry;
    struct fuse_args *args;
    refcount_t count;
    long unsigned int flags;
    struct (anon) in;
    struct (anon) out;
    wait_queue_head_t waitq;
    void *argbuf;
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
<b>Field type changed. </b>
<code>atomic_t count</code> ➡️ <code>refcount_t count</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 intr_unique</code>
</li>
</ul>
</details>
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
<code>struct fuse_args *args</code>
</li>
<li>
<b>Field added. </b>
<code>void *argbuf</code>
</li>
<li>
<b>Field removed. </b>
<code>union (anon) misc</code>
</li>
<li>
<b>Field removed. </b>
<code>struct page **pages</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fuse_page_desc *page_descs</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int max_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>struct page * inline_pages[1]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fuse_page_desc inline_page_descs[1]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int num_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fuse_file *ff</code>
</li>
<li>
<b>Field removed. </b>
<code>struct inode *inode</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fuse_io_priv *io</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head writepages_entry</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*end)(struct fuse_conn *, struct fuse_req *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct file *stolen_file</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fuse_in in</code> ➡️ <code>struct (anon) in</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fuse_out out</code> ➡️ <code>struct (anon) out</code>
</li>
</ul>
</details>
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
<code>struct fuse_mount *fm</code>
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
