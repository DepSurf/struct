# Struct: <code>devlink_linecard</code>

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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct devlink_linecard {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    refcount_t refcount;
    const struct devlink_linecard_ops *ops;
    void *priv;
    enum devlink_linecard_state state;
    struct mutex state_lock;
    const char *type;
    struct devlink_linecard_type *types;
    unsigned int types_count;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct devlink_linecard {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    refcount_t refcount;
    const struct devlink_linecard_ops *ops;
    void *priv;
    enum devlink_linecard_state state;
    struct mutex state_lock;
    const char *type;
    struct devlink_linecard_type *types;
    unsigned int types_count;
    struct devlink *nested_devlink;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devlink_linecard {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    const struct devlink_linecard_ops *ops;
    void *priv;
    enum devlink_linecard_state state;
    struct mutex state_lock;
    const char *type;
    struct devlink_linecard_type *types;
    unsigned int types_count;
    struct devlink *nested_devlink;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devlink_linecard {
    struct list_head list;
    struct devlink *devlink;
    unsigned int index;
    const struct devlink_linecard_ops *ops;
    void *priv;
    enum devlink_linecard_state state;
    struct mutex state_lock;
    const char *type;
    struct devlink_linecard_type *types;
    unsigned int types_count;
    u32 rel_index;
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
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct devlink *nested_devlink</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>refcount_t refcount</code>
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
<li>
<b>Field removed. </b>
<code>struct devlink *nested_devlink</code>
</li>
</ul>
</details>
</li>
</ul>
