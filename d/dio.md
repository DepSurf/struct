# Struct: <code>dio</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dio {
    int flags;
    int rw;
    blk_qc_t bio_cookie;
    struct block_device *bio_bdev;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct block_device *bio_bdev;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct block_device *bio_bdev;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct block_device *bio_bdev;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dio {
    int flags;
    blk_opf_t opf;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dio {
    int flags;
    blk_opf_t opf;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    bool is_pinned;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dio {
    int flags;
    blk_opf_t opf;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    bool is_pinned;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
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
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
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
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dio {
    int flags;
    int op;
    int op_flags;
    blk_qc_t bio_cookie;
    struct gendisk *bio_disk;
    struct inode *inode;
    loff_t i_size;
    dio_iodone_t *end_io;
    void *private;
    spinlock_t bio_lock;
    int page_errors;
    int is_async;
    bool defer_completion;
    bool should_dirty;
    int io_error;
    long unsigned int refcount;
    struct bio *bio_list;
    struct task_struct *waiter;
    struct kiocb *iocb;
    ssize_t result;
    struct page * pages[64];
    struct work_struct complete_work;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int op</code>
</li>
<li>
<b>Field added. </b>
<code>int op_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>int rw</code>
</li>
</ul>
</details>
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
<code>struct gendisk *bio_disk</code>
</li>
<li>
<b>Field removed. </b>
<code>struct block_device *bio_bdev</code>
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
<code>blk_qc_t bio_cookie</code>
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
<code>blk_opf_t opf</code>
</li>
<li>
<b>Field removed. </b>
<code>int op</code>
</li>
<li>
<b>Field removed. </b>
<code>int op_flags</code>
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
<code>bool is_pinned</code>
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
