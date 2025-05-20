# Struct: <code>inode_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*follow_link)(struct dentry *, void **);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    void (*put_link)(struct inode *, void *);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *);
    int (*rename2)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(struct vfsmount *, struct dentry *, struct kstat *);
    int (*setxattr)(struct dentry *, const char *, const void *, size_t, int);
    ssize_t (*getxattr)(struct dentry *, const char *, void *, size_t);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*removexattr)(struct dentry *, const char *);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t, int *);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *);
    int (*rename2)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(struct vfsmount *, struct dentry *, struct kstat *);
    int (*setxattr)(struct dentry *, struct inode *, const char *, const void *, size_t, int);
    ssize_t (*getxattr)(struct dentry *, struct inode *, const char *, void *, size_t);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*removexattr)(struct dentry *, const char *);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t, int *);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(struct vfsmount *, struct dentry *, struct kstat *);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t, int *);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t, int *);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t, int *);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t, int *);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct user_namespace *, struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct user_namespace *, struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct user_namespace *, struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct user_namespace *, struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct user_namespace *, struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct user_namespace *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct user_namespace *, struct dentry *, struct iattr *);
    int (*getattr)(struct user_namespace *, const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct user_namespace *, struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct user_namespace *, struct inode *, struct posix_acl *, int);
    int (*fileattr_set)(struct user_namespace *, struct dentry *, struct fileattr *);
    int (*fileattr_get)(struct dentry *, struct fileattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct user_namespace *, struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int, bool);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct user_namespace *, struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct user_namespace *, struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct user_namespace *, struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct user_namespace *, struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct user_namespace *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct user_namespace *, struct dentry *, struct iattr *);
    int (*getattr)(struct user_namespace *, const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct user_namespace *, struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct user_namespace *, struct inode *, struct posix_acl *, int);
    int (*fileattr_set)(struct user_namespace *, struct dentry *, struct fileattr *);
    int (*fileattr_get)(struct dentry *, struct fileattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct user_namespace *, struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int, bool);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct user_namespace *, struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct user_namespace *, struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct user_namespace *, struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct user_namespace *, struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct user_namespace *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct user_namespace *, struct dentry *, struct iattr *);
    int (*getattr)(struct user_namespace *, const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct user_namespace *, struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct user_namespace *, struct inode *, struct posix_acl *, int);
    int (*fileattr_set)(struct user_namespace *, struct dentry *, struct fileattr *);
    int (*fileattr_get)(struct dentry *, struct fileattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct user_namespace *, struct inode *, int);
    struct posix_acl * (*get_inode_acl)(struct inode *, int, bool);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct user_namespace *, struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct user_namespace *, struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct user_namespace *, struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct user_namespace *, struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct user_namespace *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct user_namespace *, struct dentry *, struct iattr *);
    int (*getattr)(struct user_namespace *, const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct user_namespace *, struct inode *, struct file *, umode_t);
    struct posix_acl * (*get_acl)(struct user_namespace *, struct dentry *, int);
    int (*set_acl)(struct user_namespace *, struct dentry *, struct posix_acl *, int);
    int (*fileattr_set)(struct user_namespace *, struct dentry *, struct fileattr *);
    int (*fileattr_get)(struct dentry *, struct fileattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct mnt_idmap *, struct inode *, int);
    struct posix_acl * (*get_inode_acl)(struct inode *, int, bool);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct mnt_idmap *, struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct mnt_idmap *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct mnt_idmap *, struct dentry *, struct iattr *);
    int (*getattr)(struct mnt_idmap *, const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct mnt_idmap *, struct inode *, struct file *, umode_t);
    struct posix_acl * (*get_acl)(struct mnt_idmap *, struct dentry *, int);
    int (*set_acl)(struct mnt_idmap *, struct dentry *, struct posix_acl *, int);
    int (*fileattr_set)(struct mnt_idmap *, struct dentry *, struct fileattr *);
    int (*fileattr_get)(struct dentry *, struct fileattr *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct mnt_idmap *, struct inode *, int);
    struct posix_acl * (*get_inode_acl)(struct inode *, int, bool);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct mnt_idmap *, struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct mnt_idmap *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct mnt_idmap *, struct dentry *, struct iattr *);
    int (*getattr)(struct mnt_idmap *, const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct mnt_idmap *, struct inode *, struct file *, umode_t);
    struct posix_acl * (*get_acl)(struct mnt_idmap *, struct dentry *, int);
    int (*set_acl)(struct mnt_idmap *, struct dentry *, struct posix_acl *, int);
    int (*fileattr_set)(struct mnt_idmap *, struct dentry *, struct fileattr *);
    int (*fileattr_get)(struct dentry *, struct fileattr *);
    struct offset_ctx * (*get_offset_ctx)(struct inode *);
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
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
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
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct inode_operations {
    struct dentry * (*lookup)(struct inode *, struct dentry *, unsigned int);
    const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *);
    int (*permission)(struct inode *, int);
    struct posix_acl * (*get_acl)(struct inode *, int);
    int (*readlink)(struct dentry *, char *, int);
    int (*create)(struct inode *, struct dentry *, umode_t, bool);
    int (*link)(struct dentry *, struct inode *, struct dentry *);
    int (*unlink)(struct inode *, struct dentry *);
    int (*symlink)(struct inode *, struct dentry *, const char *);
    int (*mkdir)(struct inode *, struct dentry *, umode_t);
    int (*rmdir)(struct inode *, struct dentry *);
    int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t);
    int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int);
    int (*setattr)(struct dentry *, struct iattr *);
    int (*getattr)(const struct path *, struct kstat *, u32, unsigned int);
    ssize_t (*listxattr)(struct dentry *, char *, size_t);
    int (*fiemap)(struct inode *, struct fiemap_extent_info *, u64, u64);
    int (*update_time)(struct inode *, struct timespec64 *, int);
    int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t);
    int (*tmpfile)(struct inode *, struct dentry *, umode_t);
    int (*set_acl)(struct inode *, struct posix_acl *, int);
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
<code>const char * (*get_link)(struct dentry *, struct inode *, struct delayed_call *)</code>
</li>
<li>
<b>Field removed. </b>
<code>const char * (*follow_link)(struct dentry *, void **)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*put_link)(struct inode *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*setxattr)(struct dentry *, const char *, const void *, size_t, int)</code> ➡️ <code>int (*setxattr)(struct dentry *, struct inode *, const char *, const void *, size_t, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>ssize_t (*getxattr)(struct dentry *, const char *, void *, size_t)</code> ➡️ <code>ssize_t (*getxattr)(struct dentry *, struct inode *, const char *, void *, size_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*rename2)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*setxattr)(struct dentry *, struct inode *, const char *, const void *, size_t, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>ssize_t (*getxattr)(struct dentry *, struct inode *, const char *, void *, size_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*removexattr)(struct dentry *, const char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *)</code> ➡️ <code>int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*getattr)(struct vfsmount *, struct dentry *, struct kstat *)</code> ➡️ <code>int (*getattr)(const struct path *, struct kstat *, u32, unsigned int)</code>
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
<b>Field type changed. </b>
<code>int (*update_time)(struct inode *, struct timespec *, int)</code> ➡️ <code>int (*update_time)(struct inode *, struct timespec64 *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t, int *)</code> ➡️ <code>int (*atomic_open)(struct inode *, struct dentry *, struct file *, unsigned int, umode_t)</code>
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
<code>int (*fileattr_set)(struct user_namespace *, struct dentry *, struct fileattr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fileattr_get)(struct dentry *, struct fileattr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*permission)(struct inode *, int)</code> ➡️ <code>int (*permission)(struct user_namespace *, struct inode *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*create)(struct inode *, struct dentry *, umode_t, bool)</code> ➡️ <code>int (*create)(struct user_namespace *, struct inode *, struct dentry *, umode_t, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*symlink)(struct inode *, struct dentry *, const char *)</code> ➡️ <code>int (*symlink)(struct user_namespace *, struct inode *, struct dentry *, const char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*mkdir)(struct inode *, struct dentry *, umode_t)</code> ➡️ <code>int (*mkdir)(struct user_namespace *, struct inode *, struct dentry *, umode_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*mknod)(struct inode *, struct dentry *, umode_t, dev_t)</code> ➡️ <code>int (*mknod)(struct user_namespace *, struct inode *, struct dentry *, umode_t, dev_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rename)(struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int)</code> ➡️ <code>int (*rename)(struct user_namespace *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*setattr)(struct dentry *, struct iattr *)</code> ➡️ <code>int (*setattr)(struct user_namespace *, struct dentry *, struct iattr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*getattr)(const struct path *, struct kstat *, u32, unsigned int)</code> ➡️ <code>int (*getattr)(struct user_namespace *, const struct path *, struct kstat *, u32, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*tmpfile)(struct inode *, struct dentry *, umode_t)</code> ➡️ <code>int (*tmpfile)(struct user_namespace *, struct inode *, struct dentry *, umode_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_acl)(struct inode *, struct posix_acl *, int)</code> ➡️ <code>int (*set_acl)(struct user_namespace *, struct inode *, struct posix_acl *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct posix_acl * (*get_acl)(struct inode *, int)</code> ➡️ <code>struct posix_acl * (*get_acl)(struct inode *, int, bool)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct posix_acl * (*get_inode_acl)(struct inode *, int, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct posix_acl * (*get_acl)(struct inode *, int, bool)</code> ➡️ <code>struct posix_acl * (*get_acl)(struct user_namespace *, struct dentry *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*tmpfile)(struct user_namespace *, struct inode *, struct dentry *, umode_t)</code> ➡️ <code>int (*tmpfile)(struct user_namespace *, struct inode *, struct file *, umode_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_acl)(struct user_namespace *, struct inode *, struct posix_acl *, int)</code> ➡️ <code>int (*set_acl)(struct user_namespace *, struct dentry *, struct posix_acl *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*permission)(struct user_namespace *, struct inode *, int)</code> ➡️ <code>int (*permission)(struct mnt_idmap *, struct inode *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*create)(struct user_namespace *, struct inode *, struct dentry *, umode_t, bool)</code> ➡️ <code>int (*create)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t, bool)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*symlink)(struct user_namespace *, struct inode *, struct dentry *, const char *)</code> ➡️ <code>int (*symlink)(struct mnt_idmap *, struct inode *, struct dentry *, const char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*mkdir)(struct user_namespace *, struct inode *, struct dentry *, umode_t)</code> ➡️ <code>int (*mkdir)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*mknod)(struct user_namespace *, struct inode *, struct dentry *, umode_t, dev_t)</code> ➡️ <code>int (*mknod)(struct mnt_idmap *, struct inode *, struct dentry *, umode_t, dev_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rename)(struct user_namespace *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int)</code> ➡️ <code>int (*rename)(struct mnt_idmap *, struct inode *, struct dentry *, struct inode *, struct dentry *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*setattr)(struct user_namespace *, struct dentry *, struct iattr *)</code> ➡️ <code>int (*setattr)(struct mnt_idmap *, struct dentry *, struct iattr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*getattr)(struct user_namespace *, const struct path *, struct kstat *, u32, unsigned int)</code> ➡️ <code>int (*getattr)(struct mnt_idmap *, const struct path *, struct kstat *, u32, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*tmpfile)(struct user_namespace *, struct inode *, struct file *, umode_t)</code> ➡️ <code>int (*tmpfile)(struct mnt_idmap *, struct inode *, struct file *, umode_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct posix_acl * (*get_acl)(struct user_namespace *, struct dentry *, int)</code> ➡️ <code>struct posix_acl * (*get_acl)(struct mnt_idmap *, struct dentry *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_acl)(struct user_namespace *, struct dentry *, struct posix_acl *, int)</code> ➡️ <code>int (*set_acl)(struct mnt_idmap *, struct dentry *, struct posix_acl *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*fileattr_set)(struct user_namespace *, struct dentry *, struct fileattr *)</code> ➡️ <code>int (*fileattr_set)(struct mnt_idmap *, struct dentry *, struct fileattr *)</code>
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
<code>struct offset_ctx * (*get_offset_ctx)(struct inode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*update_time)(struct inode *, struct timespec64 *, int)</code> ➡️ <code>int (*update_time)(struct inode *, int)</code>
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
