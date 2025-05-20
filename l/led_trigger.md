# Struct: <code>led_trigger</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    void (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    void (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    void (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    void (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    void (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    void (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    struct led_hw_trigger_type *trigger_type;
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    struct led_hw_trigger_type *trigger_type;
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    struct led_hw_trigger_type *trigger_type;
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    struct led_hw_trigger_type *trigger_type;
    spinlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    struct led_hw_trigger_type *trigger_type;
    spinlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    struct led_hw_trigger_type *trigger_type;
    spinlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    struct led_hw_trigger_type *trigger_type;
    spinlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
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
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
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
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct led_trigger {
    const char *name;
    int (*activate)(struct led_classdev *);
    void (*deactivate)(struct led_classdev *);
    rwlock_t leddev_list_lock;
    struct list_head led_cdevs;
    struct list_head next_trig;
    const struct attribute_group **groups;
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct attribute_group **groups</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*activate)(struct led_classdev *)</code> ➡️ <code>int (*activate)(struct led_classdev *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct led_hw_trigger_type *trigger_type</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>rwlock_t leddev_list_lock</code> ➡️ <code>spinlock_t leddev_list_lock</code>
</li>
</ul>
</details>
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
