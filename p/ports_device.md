# Struct: <code>ports_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    struct virtio_console_config config;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    struct virtio_console_config config;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
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
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
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
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ports_device {
    struct list_head list;
    struct work_struct control_work;
    struct work_struct config_work;
    struct list_head ports;
    spinlock_t ports_lock;
    spinlock_t c_ivq_lock;
    spinlock_t c_ovq_lock;
    u32 max_nr_ports;
    struct virtio_device *vdev;
    struct virtqueue *c_ivq;
    struct virtqueue *c_ovq;
    struct virtio_console_control cpkt;
    struct virtqueue **in_vqs;
    struct virtqueue **out_vqs;
    int chr_major;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct virtio_console_control cpkt</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 max_nr_ports</code>
</li>
<li>
<b>Field removed. </b>
<code>struct virtio_console_config config</code>
</li>
</ul>
</details>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
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
