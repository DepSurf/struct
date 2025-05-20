# Struct: <code>acpi_ec</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    long unsigned int gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    long unsigned int gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    long unsigned int gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool saved_busy_polling;
    unsigned int saved_polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    long unsigned int gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    unsigned int events_in_progress;
    unsigned int queries_in_progress;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    enum acpi_ec_event_state event_state;
    unsigned int events_to_process;
    unsigned int events_in_progress;
    unsigned int queries_in_progress;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    acpi_handle address_space_handler_holder;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    enum acpi_ec_event_state event_state;
    unsigned int events_to_process;
    unsigned int events_in_progress;
    unsigned int queries_in_progress;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    acpi_handle address_space_handler_holder;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    enum acpi_ec_event_state event_state;
    unsigned int events_to_process;
    unsigned int events_in_progress;
    unsigned int queries_in_progress;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    acpi_handle address_space_handler_holder;
    int gpe;
    int irq;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    enum acpi_ec_event_state event_state;
    unsigned int events_to_process;
    unsigned int events_in_progress;
    unsigned int queries_in_progress;
    bool busy_polling;
    unsigned int polling_guard;
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
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
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
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_ec {
    acpi_handle handle;
    u32 gpe;
    long unsigned int command_addr;
    long unsigned int data_addr;
    bool global_lock;
    long unsigned int flags;
    long unsigned int reference_count;
    struct mutex mutex;
    wait_queue_head_t wait;
    struct list_head list;
    struct transaction *curr;
    spinlock_t lock;
    struct work_struct work;
    long unsigned int timestamp;
    long unsigned int nr_pending_queries;
    bool busy_polling;
    unsigned int polling_guard;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool saved_busy_polling</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int saved_polling_guard</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool busy_polling</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int polling_guard</code>
</li>
<li>
<b>Field removed. </b>
<code>bool saved_busy_polling</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int saved_polling_guard</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int gpe</code> ➡️ <code>u32 gpe</code>
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
<code>int irq</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 gpe</code> ➡️ <code>int gpe</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int events_in_progress</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int queries_in_progress</code>
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
<code>enum acpi_ec_event_state event_state</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int events_to_process</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_pending_queries</code>
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
<code>acpi_handle address_space_handler_holder</code>
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
