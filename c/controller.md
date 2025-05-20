# Struct: <code>controller</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct controller {
    struct mutex ctrl_lock;
    struct pcie_device *pcie;
    struct slot *slot;
    wait_queue_head_t queue;
    u32 slot_cap;
    u16 slot_ctrl;
    struct timer_list poll_timer;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    unsigned int link_active_reporting;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct controller {
    struct mutex ctrl_lock;
    struct pcie_device *pcie;
    struct slot *slot;
    wait_queue_head_t queue;
    u32 slot_cap;
    u16 slot_ctrl;
    struct timer_list poll_timer;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    unsigned int link_active_reporting;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct controller {
    struct mutex ctrl_lock;
    struct pcie_device *pcie;
    struct slot *slot;
    wait_queue_head_t queue;
    u32 slot_cap;
    u16 slot_ctrl;
    struct timer_list poll_timer;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    unsigned int link_active_reporting;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct controller {
    struct mutex ctrl_lock;
    struct pcie_device *pcie;
    struct slot *slot;
    wait_queue_head_t queue;
    u32 slot_cap;
    u16 slot_ctrl;
    struct timer_list poll_timer;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    unsigned int link_active_reporting;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct controller {
    struct mutex ctrl_lock;
    struct pcie_device *pcie;
    struct slot *slot;
    wait_queue_head_t queue;
    u32 slot_cap;
    u16 slot_ctrl;
    struct timer_list poll_timer;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    unsigned int link_active_reporting;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct controller {
    struct mutex ctrl_lock;
    struct pcie_device *pcie;
    struct slot *slot;
    wait_queue_head_t queue;
    u32 slot_cap;
    u16 slot_ctrl;
    struct timer_list poll_timer;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    unsigned int link_active_reporting;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int depth;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int depth;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int depth;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int depth;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    unsigned int inband_presence_disabled;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int depth;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
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
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
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
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
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
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct controller {
    struct pcie_device *pcie;
    u32 slot_cap;
    u16 slot_ctrl;
    struct mutex ctrl_lock;
    long unsigned int cmd_started;
    unsigned int cmd_busy;
    wait_queue_head_t queue;
    atomic_t pending_events;
    unsigned int notification_enabled;
    unsigned int power_fault_detected;
    struct task_struct *poll_thread;
    u8 state;
    struct mutex state_lock;
    struct delayed_work button_work;
    struct hotplug_slot hotplug_slot;
    struct rw_semaphore reset_lock;
    unsigned int ist_running;
    int request_result;
    wait_queue_head_t requester;
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
<code>atomic_t pending_events</code>
</li>
<li>
<b>Field added. </b>
<code>struct task_struct *poll_thread</code>
</li>
<li>
<b>Field added. </b>
<code>u8 state</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex state_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct delayed_work button_work</code>
</li>
<li>
<b>Field added. </b>
<code>struct hotplug_slot hotplug_slot</code>
</li>
<li>
<b>Field added. </b>
<code>struct rw_semaphore reset_lock</code>
</li>
<li>
<b>Field added. </b>
<code>int request_result</code>
</li>
<li>
<b>Field added. </b>
<code>wait_queue_head_t requester</code>
</li>
<li>
<b>Field removed. </b>
<code>struct slot *slot</code>
</li>
<li>
<b>Field removed. </b>
<code>struct timer_list poll_timer</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int link_active_reporting</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int ist_running</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int inband_presence_disabled</code>
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
<code>unsigned int depth</code>
</li>
</ul>
</details>
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
