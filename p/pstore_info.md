# Struct: <code>pstore_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(u64 *, enum pstore_type_id *, int *, struct timespec *, char **, bool *, struct pstore_info *);
    int (*write)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, int, bool, size_t, struct pstore_info *);
    int (*write_buf)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, const char *, bool, size_t, struct pstore_info *);
    int (*erase)(enum pstore_type_id, u64, int, struct timespec, struct pstore_info *);
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(u64 *, enum pstore_type_id *, int *, struct timespec *, char **, bool *, ssize_t *, struct pstore_info *);
    int (*write)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, int, bool, size_t, struct pstore_info *);
    int (*write_buf)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, const char *, bool, size_t, struct pstore_info *);
    int (*erase)(enum pstore_type_id, u64, int, struct timespec, struct pstore_info *);
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(u64 *, enum pstore_type_id *, int *, struct timespec *, char **, bool *, ssize_t *, struct pstore_info *);
    int (*write)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, int, bool, size_t, struct pstore_info *);
    int (*write_buf)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, const char *, bool, size_t, struct pstore_info *);
    int (*write_buf_user)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, const char *, bool, size_t, struct pstore_info *);
    int (*erase)(enum pstore_type_id, u64, int, struct timespec, struct pstore_info *);
    void *data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    const char *name;
    spinlock_t buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    int max_reason;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
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
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
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
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pstore_info {
    struct module *owner;
    char *name;
    struct semaphore buf_lock;
    char *buf;
    size_t bufsize;
    struct mutex read_mutex;
    int flags;
    void *data;
    int (*open)(struct pstore_info *);
    int (*close)(struct pstore_info *);
    ssize_t (*read)(struct pstore_record *);
    int (*write)(struct pstore_record *);
    int (*write_user)(struct pstore_record *, const char *);
    int (*erase)(struct pstore_record *);
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
<b>Field type changed. </b>
<code>ssize_t (*read)(u64 *, enum pstore_type_id *, int *, struct timespec *, char **, bool *, struct pstore_info *)</code> ➡️ <code>ssize_t (*read)(u64 *, enum pstore_type_id *, int *, struct timespec *, char **, bool *, ssize_t *, struct pstore_info *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*write_buf_user)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, const char *, bool, size_t, struct pstore_info *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*write_user)(struct pstore_record *, const char *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*write_buf)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, const char *, bool, size_t, struct pstore_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*write_buf_user)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, const char *, bool, size_t, struct pstore_info *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>ssize_t (*read)(u64 *, enum pstore_type_id *, int *, struct timespec *, char **, bool *, ssize_t *, struct pstore_info *)</code> ➡️ <code>ssize_t (*read)(struct pstore_record *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*write)(enum pstore_type_id, enum kmsg_dump_reason, u64 *, unsigned int, int, bool, size_t, struct pstore_info *)</code> ➡️ <code>int (*write)(struct pstore_record *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*erase)(enum pstore_type_id, u64, int, struct timespec, struct pstore_info *)</code> ➡️ <code>int (*erase)(struct pstore_record *)</code>
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
<b>Field type changed. </b>
<code>spinlock_t buf_lock</code> ➡️ <code>struct semaphore buf_lock</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int max_reason</code>
</li>
<li>
<b>Field type changed. </b>
<code>char *name</code> ➡️ <code>const char *name</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>struct semaphore buf_lock</code> ➡️ <code>spinlock_t buf_lock</code>
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
