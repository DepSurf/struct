# Struct: <code>vfio_device_ops</code>

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
struct vfio_device_ops {
    char *name;
    int (*open)(void *);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    void (*request)(void *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open)(void *);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    void (*request)(void *, unsigned int);
    int (*match)(void *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open)(void *);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    void (*request)(void *, unsigned int);
    int (*match)(void *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open)(struct vfio_device *);
    void (*release)(struct vfio_device *);
    ssize_t (*read)(struct vfio_device *, char *, size_t, loff_t *);
    ssize_t (*write)(struct vfio_device *, const char *, size_t, loff_t *);
    long int (*ioctl)(struct vfio_device *, unsigned int, long unsigned int);
    int (*mmap)(struct vfio_device *, struct vm_area_struct *);
    void (*request)(struct vfio_device *, unsigned int);
    int (*match)(struct vfio_device *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open_device)(struct vfio_device *);
    void (*close_device)(struct vfio_device *);
    ssize_t (*read)(struct vfio_device *, char *, size_t, loff_t *);
    ssize_t (*write)(struct vfio_device *, const char *, size_t, loff_t *);
    long int (*ioctl)(struct vfio_device *, unsigned int, long unsigned int);
    int (*mmap)(struct vfio_device *, struct vm_area_struct *);
    void (*request)(struct vfio_device *, unsigned int);
    int (*match)(struct vfio_device *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open_device)(struct vfio_device *);
    void (*close_device)(struct vfio_device *);
    ssize_t (*read)(struct vfio_device *, char *, size_t, loff_t *);
    ssize_t (*write)(struct vfio_device *, const char *, size_t, loff_t *);
    long int (*ioctl)(struct vfio_device *, unsigned int, long unsigned int);
    int (*mmap)(struct vfio_device *, struct vm_area_struct *);
    void (*request)(struct vfio_device *, unsigned int);
    int (*match)(struct vfio_device *, char *);
    int (*device_feature)(struct vfio_device *, u32, void *, size_t);
};
```
</details>
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open)(void *);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    void (*request)(void *, unsigned int);
};
```
</details>
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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open)(void *);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    void (*request)(void *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open)(void *);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    void (*request)(void *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_device_ops {
    char *name;
    int (*open)(void *);
    void (*release)(void *);
    ssize_t (*read)(void *, char *, size_t, loff_t *);
    ssize_t (*write)(void *, const char *, size_t, loff_t *);
    long int (*ioctl)(void *, unsigned int, long unsigned int);
    int (*mmap)(void *, struct vm_area_struct *);
    void (*request)(void *, unsigned int);
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
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*match)(void *, char *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*open)(void *)</code> ➡️ <code>int (*open)(struct vfio_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*release)(void *)</code> ➡️ <code>void (*release)(struct vfio_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>ssize_t (*read)(void *, char *, size_t, loff_t *)</code> ➡️ <code>ssize_t (*read)(struct vfio_device *, char *, size_t, loff_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>ssize_t (*write)(void *, const char *, size_t, loff_t *)</code> ➡️ <code>ssize_t (*write)(struct vfio_device *, const char *, size_t, loff_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int (*ioctl)(void *, unsigned int, long unsigned int)</code> ➡️ <code>long int (*ioctl)(struct vfio_device *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*mmap)(void *, struct vm_area_struct *)</code> ➡️ <code>int (*mmap)(struct vfio_device *, struct vm_area_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*request)(void *, unsigned int)</code> ➡️ <code>void (*request)(struct vfio_device *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*match)(void *, char *)</code> ➡️ <code>int (*match)(struct vfio_device *, char *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*open_device)(struct vfio_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*close_device)(struct vfio_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*open)(struct vfio_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*release)(struct vfio_device *)</code>
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
<code>int (*device_feature)(struct vfio_device *, u32, void *, size_t)</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
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
