# Struct: <code>clock_event_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
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
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
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
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct clock_event_device {
    void (*event_handler)(struct clock_event_device *);
    int (*set_next_event)(long unsigned int, struct clock_event_device *);
    int (*set_next_ktime)(ktime_t, struct clock_event_device *);
    ktime_t next_event;
    u64 max_delta_ns;
    u64 min_delta_ns;
    u32 mult;
    u32 shift;
    enum clock_event_state state_use_accessors;
    unsigned int features;
    long unsigned int retries;
    int (*set_state_periodic)(struct clock_event_device *);
    int (*set_state_oneshot)(struct clock_event_device *);
    int (*set_state_oneshot_stopped)(struct clock_event_device *);
    int (*set_state_shutdown)(struct clock_event_device *);
    int (*tick_resume)(struct clock_event_device *);
    void (*broadcast)(const struct cpumask *);
    void (*suspend)(struct clock_event_device *);
    void (*resume)(struct clock_event_device *);
    long unsigned int min_delta_ticks;
    long unsigned int max_delta_ticks;
    const char *name;
    int rating;
    int irq;
    int bound_on;
    const struct cpumask *cpumask;
    struct list_head list;
    struct module *owner;
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
