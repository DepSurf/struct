# Struct: <code>xenbus_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    bool not_essential;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    bool not_essential;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    void (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    bool not_essential;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    void (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(const struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    bool allow_rebind;
    bool not_essential;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    void (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(const struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
    void (*reclaim_memory)(struct xenbus_device *);
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
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*freeze)(struct xenbus_device *);
    int (*thaw)(struct xenbus_device *);
    int (*restore)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
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
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xenbus_driver {
    const char *name;
    const struct xenbus_device_id *ids;
    int (*probe)(struct xenbus_device *, const struct xenbus_device_id *);
    void (*otherend_changed)(struct xenbus_device *, enum xenbus_state);
    int (*remove)(struct xenbus_device *);
    int (*suspend)(struct xenbus_device *);
    int (*resume)(struct xenbus_device *);
    int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *);
    struct device_driver driver;
    int (*read_otherend_details)(struct xenbus_device *);
    int (*is_ready)(struct xenbus_device *);
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
<code>bool allow_rebind</code>
</li>
<li>
<b>Field added. </b>
<code>void (*reclaim_memory)(struct xenbus_device *)</code>
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
<code>bool not_essential</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*remove)(struct xenbus_device *)</code> ➡️ <code>void (*remove)(struct xenbus_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*uevent)(struct xenbus_device *, struct kobj_uevent_env *)</code> ➡️ <code>int (*uevent)(const struct xenbus_device *, struct kobj_uevent_env *)</code>
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
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*freeze)(struct xenbus_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*thaw)(struct xenbus_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*restore)(struct xenbus_device *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
