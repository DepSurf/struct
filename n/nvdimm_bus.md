# Struct: <code>nvdimm_bus</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t probe_wait;
    struct module *module;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    struct mutex reconfig_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t probe_wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    struct list_head poison_list;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t probe_wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    struct list_head poison_list;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t probe_wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    struct list_head poison_list;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    spinlock_t poison_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t probe_wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t probe_wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t probe_wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
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
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
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
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvdimm_bus {
    struct nvdimm_bus_descriptor *nd_desc;
    wait_queue_head_t wait;
    struct list_head list;
    struct device dev;
    int id;
    int probe_active;
    atomic_t ioctl_active;
    struct list_head mapping_list;
    struct mutex reconfig_mutex;
    struct badrange badrange;
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
<code>struct list_head poison_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head mapping_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct module *module</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>spinlock_t poison_lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct badrange badrange</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head poison_list</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t poison_lock</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>wait_queue_head_t wait</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t ioctl_active</code>
</li>
<li>
<b>Field removed. </b>
<code>wait_queue_head_t probe_wait</code>
</li>
</ul>
</details>
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
