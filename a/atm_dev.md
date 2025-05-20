# Struct: <code>atm_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct atm_dev {
    const struct atmdev_ops *ops;
    const struct atmphy_ops *phy;
    const char *type;
    int number;
    void *dev_data;
    void *phy_data;
    long unsigned int flags;
    struct list_head local;
    struct list_head lecs;
    unsigned char esi[6];
    struct atm_cirange ci_range;
    struct k_atm_dev_stats stats;
    char signal;
    int link_rate;
    atomic_t refcnt;
    spinlock_t lock;
    struct proc_dir_entry *proc_entry;
    char *proc_name;
    struct device class_dev;
    struct list_head dev_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct atm_dev {
    const struct atmdev_ops *ops;
    const struct atmphy_ops *phy;
    const char *type;
    int number;
    void *dev_data;
    void *phy_data;
    long unsigned int flags;
    struct list_head local;
    struct list_head lecs;
    unsigned char esi[6];
    struct atm_cirange ci_range;
    struct k_atm_dev_stats stats;
    char signal;
    int link_rate;
    atomic_t refcnt;
    spinlock_t lock;
    struct proc_dir_entry *proc_entry;
    char *proc_name;
    struct device class_dev;
    struct list_head dev_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct atm_dev {
    const struct atmdev_ops *ops;
    const struct atmphy_ops *phy;
    const char *type;
    int number;
    void *dev_data;
    void *phy_data;
    long unsigned int flags;
    struct list_head local;
    struct list_head lecs;
    unsigned char esi[6];
    struct atm_cirange ci_range;
    struct k_atm_dev_stats stats;
    char signal;
    int link_rate;
    refcount_t refcnt;
    spinlock_t lock;
    struct proc_dir_entry *proc_entry;
    char *proc_name;
    struct device class_dev;
    struct list_head dev_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct atm_dev {
    const struct atmdev_ops *ops;
    const struct atmphy_ops *phy;
    const char *type;
    int number;
    void *dev_data;
    void *phy_data;
    long unsigned int flags;
    struct list_head local;
    struct list_head lecs;
    unsigned char esi[6];
    struct atm_cirange ci_range;
    struct k_atm_dev_stats stats;
    char signal;
    int link_rate;
    refcount_t refcnt;
    spinlock_t lock;
    struct proc_dir_entry *proc_entry;
    char *proc_name;
    struct device class_dev;
    struct list_head dev_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct atm_dev {
    const struct atmdev_ops *ops;
    const struct atmphy_ops *phy;
    const char *type;
    int number;
    void *dev_data;
    void *phy_data;
    long unsigned int flags;
    struct list_head local;
    struct list_head lecs;
    unsigned char esi[6];
    struct atm_cirange ci_range;
    struct k_atm_dev_stats stats;
    char signal;
    int link_rate;
    refcount_t refcnt;
    spinlock_t lock;
    struct proc_dir_entry *proc_entry;
    char *proc_name;
    struct device class_dev;
    struct list_head dev_list;
};
```
</details>
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
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t refcnt</code> ➡️ <code>refcount_t refcnt</code>
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
</ul>
