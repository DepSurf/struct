# Struct: <code>vfio_pci_ioeventfd</code>

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
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct vfio_pci_device *vdev;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
    bool test_mem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct vfio_pci_device *vdev;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
    bool test_mem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct vfio_pci_device *vdev;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
    bool test_mem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct vfio_pci_core_device *vdev;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
    bool test_mem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct vfio_pci_core_device *vdev;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
    bool test_mem;
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
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
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
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vfio_pci_ioeventfd {
    struct list_head next;
    struct virqfd *virqfd;
    void *addr;
    uint64_t data;
    loff_t pos;
    int bar;
    int count;
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
<code>struct vfio_pci_device *vdev</code>
</li>
<li>
<b>Field added. </b>
<code>bool test_mem</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>struct vfio_pci_device *vdev</code> ➡️ <code>struct vfio_pci_core_device *vdev</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
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
