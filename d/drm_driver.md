# Struct: <code>drm_driver</code>

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
struct drm_driver {
    int (*load)(struct drm_device *, long unsigned int);
    int (*open)(struct drm_device *, struct drm_file *);
    void (*postclose)(struct drm_device *, struct drm_file *);
    void (*lastclose)(struct drm_device *);
    void (*unload)(struct drm_device *);
    void (*release)(struct drm_device *);
    void (*master_set)(struct drm_device *, struct drm_file *, bool);
    void (*master_drop)(struct drm_device *, struct drm_file *);
    void (*debugfs_init)(struct drm_minor *);
    struct drm_gem_object * (*gem_create_object)(struct drm_device *, size_t);
    int (*prime_handle_to_fd)(struct drm_device *, struct drm_file *, uint32_t, uint32_t, int *);
    int (*prime_fd_to_handle)(struct drm_device *, struct drm_file *, int, uint32_t *);
    struct drm_gem_object * (*gem_prime_import)(struct drm_device *, struct dma_buf *);
    struct drm_gem_object * (*gem_prime_import_sg_table)(struct drm_device *, struct dma_buf_attachment *, struct sg_table *);
    int (*dumb_create)(struct drm_file *, struct drm_device *, struct drm_mode_create_dumb *);
    int (*dumb_map_offset)(struct drm_file *, struct drm_device *, uint32_t, uint64_t *);
    void (*show_fdinfo)(struct drm_printer *, struct drm_file *);
    int major;
    int minor;
    int patchlevel;
    char *name;
    char *desc;
    char *date;
    u32 driver_features;
    const struct drm_ioctl_desc *ioctls;
    int num_ioctls;
    const struct file_operations *fops;
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
</ul>
