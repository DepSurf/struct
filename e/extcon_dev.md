# Struct: <code>extcon_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    unsigned int id;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    unsigned int id;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
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
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
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
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct extcon_dev {
    const char *name;
    const unsigned int *supported_cable;
    const u32 *mutually_exclusive;
    struct device dev;
    struct raw_notifier_head nh_all;
    struct raw_notifier_head *nh;
    struct list_head entry;
    int max_supported;
    spinlock_t lock;
    u32 state;
    struct device_type extcon_dev_type;
    struct extcon_cable *cables;
    struct attribute_group attr_g_muex;
    struct attribute **attrs_muex;
    struct device_attribute *d_attrs_muex;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct raw_notifier_head nh_all</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int id</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
