# Struct: <code>ncsi_dev_priv</code>

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
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    spinlock_t lock;
    unsigned int inet6_addr_num;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    spinlock_t lock;
    unsigned int inet6_addr_num;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    spinlock_t lock;
    unsigned int inet6_addr_num;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    spinlock_t lock;
    unsigned int inet6_addr_num;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    spinlock_t lock;
    unsigned int inet6_addr_num;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_package *force_package;
    struct ncsi_channel *force_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int inet6_addr_num;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int inet6_addr_num;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    bool mlx_multi_host;
    u32 package_whitelist;
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
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
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
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ncsi_dev_priv {
    struct ncsi_dev ndev;
    unsigned int flags;
    unsigned int gma_flag;
    spinlock_t lock;
    unsigned int package_probe_id;
    unsigned int package_num;
    struct list_head packages;
    struct ncsi_channel *hot_channel;
    struct ncsi_request requests[256];
    unsigned int request_id;
    unsigned int pending_req_num;
    struct ncsi_package *active_package;
    struct ncsi_channel *active_channel;
    struct list_head channel_queue;
    struct work_struct work;
    struct packet_type ptype;
    struct list_head node;
    struct list_head vlan_vids;
    bool multi_package;
    u32 package_whitelist;
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
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ncsi_channel *hot_channel</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head vlan_vids</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ncsi_package *force_package</code>
</li>
<li>
<b>Field added. </b>
<code>struct ncsi_channel *force_channel</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int gma_flag</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int package_probe_id</code>
</li>
<li>
<b>Field added. </b>
<code>bool multi_package</code>
</li>
<li>
<b>Field added. </b>
<code>u32 package_whitelist</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ncsi_package *force_package</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ncsi_channel *force_channel</code>
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
<b>Field removed. </b>
<code>unsigned int inet6_addr_num</code>
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
<code>bool mlx_multi_host</code>
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
