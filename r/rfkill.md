# Struct: <code>rfkill</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    long unsigned int hard_block_reasons;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    long unsigned int hard_block_reasons;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    long unsigned int hard_block_reasons;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    long unsigned int hard_block_reasons;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    long unsigned int hard_block_reasons;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    long unsigned int hard_block_reasons;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    long unsigned int hard_block_reasons;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    bool need_sync;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
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
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
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
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rfkill {
    spinlock_t lock;
    enum rfkill_type type;
    long unsigned int state;
    u32 idx;
    bool registered;
    bool persistent;
    bool polling_paused;
    bool suspended;
    const struct rfkill_ops *ops;
    void *data;
    struct led_trigger led_trigger;
    const char *ledtrigname;
    struct device dev;
    struct list_head node;
    struct delayed_work poll_work;
    struct work_struct uevent_work;
    struct work_struct sync_work;
    char name[0];
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
<code>bool polling_paused</code>
</li>
<li>
<b>Field added. </b>
<code>bool suspended</code>
</li>
</ul>
</details>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int hard_block_reasons</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool need_sync</code>
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
