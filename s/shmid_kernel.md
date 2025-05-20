# Struct: <code>shmid_kernel</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time_t shm_atim;
    time_t shm_dtim;
    time_t shm_ctim;
    pid_t shm_cprid;
    pid_t shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time_t shm_atim;
    time_t shm_dtim;
    time_t shm_ctim;
    pid_t shm_cprid;
    pid_t shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time_t shm_atim;
    time_t shm_dtim;
    time_t shm_ctim;
    pid_t shm_cprid;
    pid_t shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time_t shm_atim;
    time_t shm_dtim;
    time_t shm_ctim;
    pid_t shm_cprid;
    pid_t shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    pid_t shm_cprid;
    pid_t shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct ucounts *mlock_ucounts;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
    struct ipc_namespace *ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct ucounts *mlock_ucounts;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
    struct ipc_namespace *ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct ucounts *mlock_ucounts;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
    struct ipc_namespace *ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct ucounts *mlock_ucounts;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
    struct ipc_namespace *ns;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct ucounts *mlock_ucounts;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
    struct ipc_namespace *ns;
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
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
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
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct shmid_kernel {
    struct kern_ipc_perm shm_perm;
    struct file *shm_file;
    long unsigned int shm_nattch;
    long unsigned int shm_segsz;
    time64_t shm_atim;
    time64_t shm_dtim;
    time64_t shm_ctim;
    struct pid *shm_cprid;
    struct pid *shm_lprid;
    struct user_struct *mlock_user;
    struct task_struct *shm_creator;
    struct list_head shm_clist;
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>time_t shm_atim</code> ➡️ <code>time64_t shm_atim</code>
</li>
<li>
<b>Field type changed. </b>
<code>time_t shm_dtim</code> ➡️ <code>time64_t shm_dtim</code>
</li>
<li>
<b>Field type changed. </b>
<code>time_t shm_ctim</code> ➡️ <code>time64_t shm_ctim</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>pid_t shm_cprid</code> ➡️ <code>struct pid *shm_cprid</code>
</li>
<li>
<b>Field type changed. </b>
<code>pid_t shm_lprid</code> ➡️ <code>struct pid *shm_lprid</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ucounts *mlock_ucounts</code>
</li>
<li>
<b>Field added. </b>
<code>struct ipc_namespace *ns</code>
</li>
<li>
<b>Field removed. </b>
<code>struct user_struct *mlock_user</code>
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
