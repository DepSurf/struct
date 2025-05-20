# Struct: <code>fuse_fs_context</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool legacy_opts_show;
    bool dax;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    struct dax_device *dax_dev;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool legacy_opts_show;
    bool dax;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    struct dax_device *dax_dev;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    struct file *file;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool legacy_opts_show;
    bool dax;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    struct dax_device *dax_dev;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    struct file *file;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool legacy_opts_show;
    enum fuse_dax_mode dax_mode;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    struct dax_device *dax_dev;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    struct file *file;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool legacy_opts_show;
    enum fuse_dax_mode dax_mode;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    struct dax_device *dax_dev;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    struct file *file;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool legacy_opts_show;
    enum fuse_dax_mode dax_mode;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    struct dax_device *dax_dev;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    struct file *file;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool legacy_opts_show;
    enum fuse_dax_mode dax_mode;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    struct dax_device *dax_dev;
    void **fudptr;
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
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
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
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fuse_fs_context {
    int fd;
    unsigned int rootmode;
    kuid_t user_id;
    kgid_t group_id;
    bool is_bdev;
    bool fd_present;
    bool rootmode_present;
    bool user_id_present;
    bool group_id_present;
    bool default_permissions;
    bool allow_other;
    bool destroy;
    bool no_control;
    bool no_force_umount;
    bool no_mount_options;
    unsigned int max_read;
    unsigned int blksize;
    const char *subtype;
    void **fudptr;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool legacy_opts_show</code>
</li>
<li>
<b>Field added. </b>
<code>bool dax</code>
</li>
<li>
<b>Field added. </b>
<code>struct dax_device *dax_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>bool no_mount_options</code>
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
<code>struct file *file</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum fuse_dax_mode dax_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>bool dax</code>
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
