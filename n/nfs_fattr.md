# Struct: <code>nfs_fattr</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec64 pre_mtime;
    struct timespec64 pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
    struct nfs4_label *label;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec64 pre_mtime;
    struct timespec64 pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
    struct nfs4_label *label;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec64 pre_mtime;
    struct timespec64 pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
    struct nfs4_label *label;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec64 pre_mtime;
    struct timespec64 pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
    struct nfs4_label *label;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec64 pre_mtime;
    struct timespec64 pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
    struct nfs4_label *label;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec64 atime;
    struct timespec64 mtime;
    struct timespec64 ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec64 pre_mtime;
    struct timespec64 pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
    struct nfs4_label *label;
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
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
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
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nfs_fattr {
    unsigned int valid;
    umode_t mode;
    __u32 nlink;
    kuid_t uid;
    kgid_t gid;
    dev_t rdev;
    __u64 size;
    union (anon) du;
    struct nfs_fsid fsid;
    __u64 fileid;
    __u64 mounted_on_fileid;
    struct timespec atime;
    struct timespec mtime;
    struct timespec ctime;
    __u64 change_attr;
    __u64 pre_change_attr;
    __u64 pre_size;
    struct timespec pre_mtime;
    struct timespec pre_ctime;
    long unsigned int time_start;
    long unsigned int gencount;
    struct nfs4_string *owner_name;
    struct nfs4_string *group_name;
    struct nfs4_threshold *mdsthreshold;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
