# Struct: <code>cftype</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
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
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
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
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cftype {
    char name[64];
    long unsigned int private;
    size_t max_write_len;
    unsigned int flags;
    unsigned int file_offset;
    struct cgroup_subsys *ss;
    struct list_head node;
    struct kernfs_ops *kf_ops;
    int (*open)(struct kernfs_open_file *);
    void (*release)(struct kernfs_open_file *);
    u64 (*read_u64)(struct cgroup_subsys_state *, struct cftype *);
    s64 (*read_s64)(struct cgroup_subsys_state *, struct cftype *);
    int (*seq_show)(struct seq_file *, void *);
    void * (*seq_start)(struct seq_file *, loff_t *);
    void * (*seq_next)(struct seq_file *, void *, loff_t *);
    void (*seq_stop)(struct seq_file *, void *);
    int (*write_u64)(struct cgroup_subsys_state *, struct cftype *, u64);
    int (*write_s64)(struct cgroup_subsys_state *, struct cftype *, s64);
    ssize_t (*write)(struct kernfs_open_file *, char *, size_t, loff_t);
    __poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *);
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
<code>int (*open)(struct kernfs_open_file *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*release)(struct kernfs_open_file *)</code>
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__poll_t (*poll)(struct kernfs_open_file *, struct poll_table_struct *)</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
