# Struct: <code>iommu_group</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
    struct list_head entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
    struct list_head entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
    struct list_head entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
    struct list_head entry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *blocking_domain;
    struct iommu_domain *domain;
    struct list_head entry;
    unsigned int owner_cnt;
    void *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct xarray pasid_array;
    struct mutex mutex;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *blocking_domain;
    struct iommu_domain *domain;
    struct list_head entry;
    unsigned int owner_cnt;
    void *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct xarray pasid_array;
    struct mutex mutex;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *blocking_domain;
    struct iommu_domain *domain;
    struct list_head entry;
    unsigned int owner_cnt;
    void *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct xarray pasid_array;
    struct mutex mutex;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *blocking_domain;
    struct iommu_domain *domain;
    struct list_head entry;
    unsigned int owner_cnt;
    void *owner;
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
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct iommu_group {
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
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iommu_group {
    struct kobject kobj;
    struct kobject *devices_kobj;
    struct list_head devices;
    struct mutex mutex;
    struct blocking_notifier_head notifier;
    void *iommu_data;
    void (*iommu_data_release)(void *);
    char *name;
    int id;
    struct iommu_domain *default_domain;
    struct iommu_domain *domain;
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head entry</code>
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct iommu_domain *blocking_domain</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int owner_cnt</code>
</li>
<li>
<b>Field added. </b>
<code>void *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>struct blocking_notifier_head notifier</code>
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
<code>struct xarray pasid_array</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct kobject kobj</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kobject *devices_kobj</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head devices</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex mutex</code>
</li>
<li>
<b>Field removed. </b>
<code>struct blocking_notifier_head notifier</code>
</li>
<li>
<b>Field removed. </b>
<code>void *iommu_data</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*iommu_data_release)(void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>char *name</code>
</li>
<li>
<b>Field removed. </b>
<code>int id</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iommu_domain *default_domain</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iommu_domain *domain</code>
</li>
</ul>
</details>
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
