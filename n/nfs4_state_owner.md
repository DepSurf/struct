# Struct: <code>nfs4_state_owner</code>

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
struct nfs4_state_owner {
    struct nfs_server *so_server;
    struct list_head so_lru;
    long unsigned int so_expires;
    struct rb_node so_server_node;
    const struct cred *so_cred;
    spinlock_t so_lock;
    atomic_t so_count;
    long unsigned int so_flags;
    struct list_head so_states;
    struct nfs_seqid_counter so_seqid;
    seqcount_spinlock_t so_reclaim_seqcount;
    struct mutex so_delegreturn_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nfs4_state_owner {
    struct nfs_server *so_server;
    struct list_head so_lru;
    long unsigned int so_expires;
    struct rb_node so_server_node;
    const struct cred *so_cred;
    spinlock_t so_lock;
    atomic_t so_count;
    long unsigned int so_flags;
    struct list_head so_states;
    struct nfs_seqid_counter so_seqid;
    seqcount_spinlock_t so_reclaim_seqcount;
    struct mutex so_delegreturn_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nfs4_state_owner {
    struct nfs_server *so_server;
    struct list_head so_lru;
    long unsigned int so_expires;
    struct rb_node so_server_node;
    const struct cred *so_cred;
    spinlock_t so_lock;
    atomic_t so_count;
    long unsigned int so_flags;
    struct list_head so_states;
    struct nfs_seqid_counter so_seqid;
    seqcount_spinlock_t so_reclaim_seqcount;
    struct mutex so_delegreturn_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nfs4_state_owner {
    struct nfs_server *so_server;
    struct list_head so_lru;
    long unsigned int so_expires;
    struct rb_node so_server_node;
    const struct cred *so_cred;
    spinlock_t so_lock;
    atomic_t so_count;
    long unsigned int so_flags;
    struct list_head so_states;
    struct nfs_seqid_counter so_seqid;
    seqcount_spinlock_t so_reclaim_seqcount;
    struct mutex so_delegreturn_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nfs4_state_owner {
    struct nfs_server *so_server;
    struct list_head so_lru;
    long unsigned int so_expires;
    struct rb_node so_server_node;
    const struct cred *so_cred;
    spinlock_t so_lock;
    atomic_t so_count;
    long unsigned int so_flags;
    struct list_head so_states;
    struct nfs_seqid_counter so_seqid;
    seqcount_spinlock_t so_reclaim_seqcount;
    struct mutex so_delegreturn_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nfs4_state_owner {
    struct nfs_server *so_server;
    struct list_head so_lru;
    long unsigned int so_expires;
    struct rb_node so_server_node;
    const struct cred *so_cred;
    spinlock_t so_lock;
    atomic_t so_count;
    long unsigned int so_flags;
    struct list_head so_states;
    struct nfs_seqid_counter so_seqid;
    seqcount_spinlock_t so_reclaim_seqcount;
    struct mutex so_delegreturn_mutex;
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
