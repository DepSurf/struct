# Struct: <code>drm_file</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
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
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool was_master;
    bool is_master;
    bool supports_virtualized_cursor_plane;
    struct drm_master *master;
    spinlock_t master_lookup_lock;
    struct pid *pid;
    u64 client_id;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
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
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
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
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_file {
    bool authenticated;
    bool stereo_allowed;
    bool universal_planes;
    bool atomic;
    bool aspect_ratio_allowed;
    bool writeback_connectors;
    bool is_master;
    struct drm_master *master;
    struct pid *pid;
    drm_magic_t magic;
    struct list_head lhead;
    struct drm_minor *minor;
    struct idr object_idr;
    spinlock_t table_lock;
    struct idr syncobj_idr;
    spinlock_t syncobj_table_lock;
    struct file *filp;
    void *driver_priv;
    struct list_head fbs;
    struct mutex fbs_lock;
    struct list_head blobs;
    wait_queue_head_t event_wait;
    struct list_head pending_event_list;
    struct list_head event_list;
    int event_space;
    struct mutex event_read_lock;
    struct drm_prime_file_private prime;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
