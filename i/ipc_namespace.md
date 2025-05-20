# Struct: <code>ipc_namespace</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ipc_namespace {
    atomic_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ipc_namespace {
    atomic_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ipc_namespace {
    atomic_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ipc_namespace {
    atomic_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ipc_namespace {
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ipc_namespace {
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ipc_namespace {
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ipc_namespace {
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct ctl_table_set mq_set;
    struct ctl_table_header *mq_sysctls;
    struct ctl_table_set ipc_set;
    struct ctl_table_header *ipc_sysctls;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ipc_namespace {
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    struct percpu_counter percpu_msg_bytes;
    struct percpu_counter percpu_msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct ctl_table_set mq_set;
    struct ctl_table_header *mq_sysctls;
    struct ctl_table_set ipc_set;
    struct ctl_table_header *ipc_sysctls;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ipc_namespace {
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    struct percpu_counter percpu_msg_bytes;
    struct percpu_counter percpu_msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct ctl_table_set mq_set;
    struct ctl_table_header *mq_sysctls;
    struct ctl_table_set ipc_set;
    struct ctl_table_header *ipc_sysctls;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ipc_namespace {
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    struct percpu_counter percpu_msg_bytes;
    struct percpu_counter percpu_msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct ctl_table_set mq_set;
    struct ctl_table_header *mq_sysctls;
    struct ctl_table_set ipc_set;
    struct ctl_table_header *ipc_sysctls;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct llist_node mnt_llist;
    struct ns_common ns;
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
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
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
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ipc_namespace {
    refcount_t count;
    struct ipc_ids ids[3];
    int sem_ctls[4];
    int used_sems;
    unsigned int msg_ctlmax;
    unsigned int msg_ctlmnb;
    unsigned int msg_ctlmni;
    atomic_t msg_bytes;
    atomic_t msg_hdrs;
    size_t shm_ctlmax;
    size_t shm_ctlall;
    long unsigned int shm_tot;
    int shm_ctlmni;
    int shm_rmid_forced;
    struct notifier_block ipcns_nb;
    struct vfsmount *mq_mnt;
    unsigned int mq_queues_count;
    unsigned int mq_queues_max;
    unsigned int mq_msg_max;
    unsigned int mq_msgsize_max;
    unsigned int mq_msg_default;
    unsigned int mq_msgsize_default;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct ns_common ns;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ucounts *ucounts</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t count</code> ➡️ <code>refcount_t count</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct llist_node mnt_llist</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>refcount_t count</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ctl_table_set mq_set</code>
</li>
<li>
<b>Field added. </b>
<code>struct ctl_table_header *mq_sysctls</code>
</li>
<li>
<b>Field added. </b>
<code>struct ctl_table_set ipc_set</code>
</li>
<li>
<b>Field added. </b>
<code>struct ctl_table_header *ipc_sysctls</code>
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
<code>struct percpu_counter percpu_msg_bytes</code>
</li>
<li>
<b>Field added. </b>
<code>struct percpu_counter percpu_msg_hdrs</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t msg_bytes</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t msg_hdrs</code>
</li>
</ul>
</details>
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
