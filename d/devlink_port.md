# Struct: <code>devlink_port</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    bool split;
    u32 split_group;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    bool split;
    u32 split_group;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct list_head region_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    u8 attrs_set;
    u8 switch_port;
    struct delayed_work type_warn_dw;
    struct list_head reporter_list;
    struct mutex reporters_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct list_head region_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    u8 attrs_set;
    u8 switch_port;
    struct delayed_work type_warn_dw;
    struct list_head reporter_list;
    struct mutex reporters_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct list_head region_list;
    struct devlink *devlink;
    unsigned int index;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    u8 attrs_set;
    u8 switch_port;
    struct delayed_work type_warn_dw;
    struct list_head reporter_list;
    struct mutex reporters_lock;
    struct devlink_rate *devlink_rate;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct list_head region_list;
    struct devlink *devlink;
    unsigned int index;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    u8 attrs_set;
    u8 switch_port;
    struct delayed_work type_warn_dw;
    struct list_head reporter_list;
    struct mutex reporters_lock;
    struct devlink_rate *devlink_rate;
    struct devlink_linecard *linecard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head region_list;
    struct devlink *devlink;
    unsigned int index;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    struct (anon) type_eth;
    struct (anon) type_ib;
    struct devlink_port_attrs attrs;
    u8 attrs_set;
    u8 switch_port;
    u8 registered;
    u8 initialized;
    struct delayed_work type_warn_dw;
    struct list_head reporter_list;
    struct mutex reporters_lock;
    struct devlink_rate *devlink_rate;
    struct devlink_linecard *linecard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head region_list;
    struct devlink *devlink;
    const struct devlink_port_ops *ops;
    unsigned int index;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    struct (anon) type_eth;
    struct (anon) type_ib;
    struct devlink_port_attrs attrs;
    u8 attrs_set;
    u8 switch_port;
    u8 registered;
    u8 initialized;
    struct delayed_work type_warn_dw;
    struct list_head reporter_list;
    struct devlink_rate *devlink_rate;
    struct devlink_linecard *linecard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head region_list;
    struct devlink *devlink;
    const struct devlink_port_ops *ops;
    unsigned int index;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    struct (anon) type_eth;
    struct (anon) type_ib;
    struct devlink_port_attrs attrs;
    u8 attrs_set;
    u8 switch_port;
    u8 registered;
    u8 initialized;
    struct delayed_work type_warn_dw;
    struct list_head reporter_list;
    struct devlink_rate *devlink_rate;
    struct devlink_linecard *linecard;
    u32 rel_index;
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
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
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
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct devlink_port {
    struct list_head list;
    struct list_head param_list;
    struct devlink *devlink;
    unsigned int index;
    bool registered;
    spinlock_t type_lock;
    enum devlink_port_type type;
    enum devlink_port_type desired_type;
    void *type_dev;
    struct devlink_port_attrs attrs;
    struct delayed_work type_warn_dw;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct devlink_port_attrs attrs</code>
</li>
<li>
<b>Field removed. </b>
<code>bool split</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 split_group</code>
</li>
</ul>
</details>
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
<code>struct list_head param_list</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t type_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct delayed_work type_warn_dw</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head region_list</code>
</li>
<li>
<b>Field added. </b>
<code>u8 attrs_set</code>
</li>
<li>
<b>Field added. </b>
<code>u8 switch_port</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head reporter_list</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex reporters_lock</code>
</li>
</ul>
</details>
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
<code>struct devlink_rate *devlink_rate</code>
</li>
<li>
<b>Field removed. </b>
<code>bool registered</code>
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
<code>struct devlink_linecard *linecard</code>
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
<code>struct (anon) type_eth</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) type_ib</code>
</li>
<li>
<b>Field added. </b>
<code>u8 registered</code>
</li>
<li>
<b>Field added. </b>
<code>u8 initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head param_list</code>
</li>
<li>
<b>Field removed. </b>
<code>void *type_dev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct devlink_port_ops *ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mutex reporters_lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 rel_index</code>
</li>
</ul>
</details>
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
