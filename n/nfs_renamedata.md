# Struct: <code>nfs_renamedata</code>

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
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
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
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_task task;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_task task;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_task task;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    struct rpc_task task;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
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
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
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
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nfs_renamedata {
    struct nfs_renameargs args;
    struct nfs_renameres res;
    const struct cred *cred;
    struct inode *old_dir;
    struct dentry *old_dentry;
    struct nfs_fattr old_fattr;
    struct inode *new_dir;
    struct dentry *new_dentry;
    struct nfs_fattr new_fattr;
    void (*complete)(struct rpc_task *, struct nfs_renamedata *);
    long int timeout;
    bool cancelled;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool cancelled</code>
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
<code>struct rpc_cred *cred</code> ➡️ <code>const struct cred *cred</code>
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rpc_task task</code>
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
