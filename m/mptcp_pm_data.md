# Struct: <code>mptcp_pm_data</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    spinlock_t lock;
    bool addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 subflows;
    u8 add_addr_signal_max;
    u8 add_addr_accept_max;
    u8 local_addr_max;
    u8 subflows_max;
    u8 status;
    struct work_struct work;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    struct list_head anno_list;
    spinlock_t lock;
    u8 addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 subflows;
    u8 add_addr_signal_max;
    u8 add_addr_accept_max;
    u8 local_addr_max;
    u8 subflows_max;
    u8 status;
    u8 rm_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    struct list_head anno_list;
    spinlock_t lock;
    u8 addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 subflows;
    u8 status;
    struct mptcp_rm_list rm_list_tx;
    struct mptcp_rm_list rm_list_rx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    struct list_head anno_list;
    spinlock_t lock;
    u8 addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    bool remote_deny_join_id0;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 subflows;
    u8 status;
    struct mptcp_rm_list rm_list_tx;
    struct mptcp_rm_list rm_list_rx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    struct list_head anno_list;
    struct list_head userspace_pm_local_addr_list;
    spinlock_t lock;
    u8 addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    bool remote_deny_join_id0;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 pm_type;
    u8 subflows;
    u8 status;
    long unsigned int id_avail_bitmap[4];
    struct mptcp_rm_list rm_list_tx;
    struct mptcp_rm_list rm_list_rx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    struct list_head anno_list;
    struct list_head userspace_pm_local_addr_list;
    spinlock_t lock;
    u8 addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    bool remote_deny_join_id0;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 pm_type;
    u8 subflows;
    u8 status;
    long unsigned int id_avail_bitmap[4];
    struct mptcp_rm_list rm_list_tx;
    struct mptcp_rm_list rm_list_rx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    struct list_head anno_list;
    struct list_head userspace_pm_local_addr_list;
    spinlock_t lock;
    u8 addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    bool remote_deny_join_id0;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 pm_type;
    u8 subflows;
    u8 status;
    long unsigned int id_avail_bitmap[4];
    struct mptcp_rm_list rm_list_tx;
    struct mptcp_rm_list rm_list_rx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mptcp_pm_data {
    struct mptcp_addr_info local;
    struct mptcp_addr_info remote;
    struct list_head anno_list;
    struct list_head userspace_pm_local_addr_list;
    spinlock_t lock;
    u8 addr_signal;
    bool server_side;
    bool work_pending;
    bool accept_addr;
    bool accept_subflow;
    bool remote_deny_join_id0;
    u8 add_addr_signaled;
    u8 add_addr_accepted;
    u8 local_addr_used;
    u8 pm_type;
    u8 subflows;
    u8 status;
    long unsigned int id_avail_bitmap[4];
    struct mptcp_rm_list rm_list_tx;
    struct mptcp_rm_list rm_list_rx;
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head anno_list</code>
</li>
<li>
<b>Field added. </b>
<code>u8 rm_id</code>
</li>
<li>
<b>Field removed. </b>
<code>struct work_struct work</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool addr_signal</code> ➡️ <code>u8 addr_signal</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mptcp_rm_list rm_list_tx</code>
</li>
<li>
<b>Field added. </b>
<code>struct mptcp_rm_list rm_list_rx</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 add_addr_signal_max</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 add_addr_accept_max</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 local_addr_max</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 subflows_max</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 rm_id</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool remote_deny_join_id0</code>
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
<code>struct list_head userspace_pm_local_addr_list</code>
</li>
<li>
<b>Field added. </b>
<code>u8 pm_type</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int id_avail_bitmap[4]</code>
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
