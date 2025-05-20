# Struct: <code>nfs4_mig_recovery_ops</code>

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
In <code>5.4</code>: Absent ⚠️
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
struct nfs4_mig_recovery_ops {
    int (*get_locations)(struct inode *, struct nfs4_fs_locations *, struct page *, const struct cred *);
    int (*fsid_present)(struct inode *, const struct cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nfs4_mig_recovery_ops {
    int (*get_locations)(struct nfs_server *, struct nfs_fh *, struct nfs4_fs_locations *, struct page *, const struct cred *);
    int (*fsid_present)(struct inode *, const struct cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nfs4_mig_recovery_ops {
    int (*get_locations)(struct nfs_server *, struct nfs_fh *, struct nfs4_fs_locations *, struct page *, const struct cred *);
    int (*fsid_present)(struct inode *, const struct cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nfs4_mig_recovery_ops {
    int (*get_locations)(struct nfs_server *, struct nfs_fh *, struct nfs4_fs_locations *, struct page *, const struct cred *);
    int (*fsid_present)(struct inode *, const struct cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nfs4_mig_recovery_ops {
    int (*get_locations)(struct nfs_server *, struct nfs_fh *, struct nfs4_fs_locations *, struct page *, const struct cred *);
    int (*fsid_present)(struct inode *, const struct cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nfs4_mig_recovery_ops {
    int (*get_locations)(struct nfs_server *, struct nfs_fh *, struct nfs4_fs_locations *, struct page *, const struct cred *);
    int (*fsid_present)(struct inode *, const struct cred *);
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*get_locations)(struct inode *, struct nfs4_fs_locations *, struct page *, const struct cred *)</code> ➡️ <code>int (*get_locations)(struct nfs_server *, struct nfs_fh *, struct nfs4_fs_locations *, struct page *, const struct cred *)</code>
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
