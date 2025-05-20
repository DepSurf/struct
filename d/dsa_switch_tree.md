# Struct: <code>dsa_switch_tree</code>

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
struct dsa_switch_tree {
    struct list_head list;
    u32 tree;
    struct kref refcount;
    bool applied;
    struct dsa_platform_data *pd;
    struct net_device *master_netdev;
    int (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *, struct net_device *);
    struct ethtool_ops master_ethtool_ops;
    const struct ethtool_ops *master_orig_ethtool_ops;
    s8 cpu_switch;
    s8 cpu_port;
    struct dsa_switch * ds[4];
    const struct dsa_device_ops *tag_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    u32 tree;
    struct kref refcount;
    bool applied;
    struct dsa_platform_data *pd;
    struct net_device *master_netdev;
    int (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *, struct net_device *);
    struct ethtool_ops master_ethtool_ops;
    const struct ethtool_ops *master_orig_ethtool_ops;
    s8 cpu_switch;
    s8 cpu_port;
    struct dsa_switch * ds[4];
    const struct dsa_device_ops *tag_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    u32 tree;
    struct kref refcount;
    bool applied;
    struct dsa_platform_data *pd;
    struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *, struct net_device *);
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
    const struct dsa_device_ops *tag_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct list_head ports;
    struct list_head rtable;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct list_head ports;
    struct list_head rtable;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    const struct dsa_device_ops *tag_ops;
    enum dsa_tag_protocol default_proto;
    struct dsa_platform_data *pd;
    struct list_head ports;
    struct list_head rtable;
    struct net_device **lags;
    unsigned int lags_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    const struct dsa_device_ops *tag_ops;
    enum dsa_tag_protocol default_proto;
    struct dsa_platform_data *pd;
    struct list_head ports;
    struct list_head rtable;
    struct net_device **lags;
    unsigned int lags_len;
    unsigned int last_switch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct list_head ports;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    struct dsa_lag **lags;
    const struct dsa_device_ops *tag_ops;
    enum dsa_tag_protocol default_proto;
    bool setup;
    struct dsa_platform_data *pd;
    struct list_head rtable;
    unsigned int lags_len;
    unsigned int last_switch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct list_head ports;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    struct dsa_lag **lags;
    const struct dsa_device_ops *tag_ops;
    enum dsa_tag_protocol default_proto;
    bool setup;
    struct dsa_platform_data *pd;
    struct list_head rtable;
    unsigned int lags_len;
    unsigned int last_switch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct list_head ports;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    struct dsa_lag **lags;
    const struct dsa_device_ops *tag_ops;
    enum dsa_tag_protocol default_proto;
    bool setup;
    struct dsa_platform_data *pd;
    struct list_head rtable;
    unsigned int lags_len;
    unsigned int last_switch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct list_head ports;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    struct dsa_lag **lags;
    const struct dsa_device_ops *tag_ops;
    enum dsa_tag_protocol default_proto;
    bool setup;
    struct dsa_platform_data *pd;
    struct list_head rtable;
    unsigned int lags_len;
    unsigned int last_switch;
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
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
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
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dsa_switch_tree {
    struct list_head list;
    struct raw_notifier_head nh;
    unsigned int index;
    struct kref refcount;
    bool setup;
    struct dsa_platform_data *pd;
    struct dsa_port *cpu_dp;
    struct dsa_switch * ds[4];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct raw_notifier_head nh</code>
</li>
<li>
<b>Field added. </b>
<code>struct dsa_port *cpu_dp</code>
</li>
<li>
<b>Field removed. </b>
<code>struct net_device *master_netdev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ethtool_ops master_ethtool_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct ethtool_ops *master_orig_ethtool_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>s8 cpu_switch</code>
</li>
<li>
<b>Field removed. </b>
<code>s8 cpu_port</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *, struct net_device *)</code> ➡️ <code>struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *, struct net_device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int index</code>
</li>
<li>
<b>Field added. </b>
<code>bool setup</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 tree</code>
</li>
<li>
<b>Field removed. </b>
<code>bool applied</code>
</li>
<li>
<b>Field removed. </b>
<code>struct sk_buff * (*rcv)(struct sk_buff *, struct net_device *, struct packet_type *, struct net_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct dsa_device_ops *tag_ops</code>
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
<code>struct list_head ports</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head rtable</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dsa_port *cpu_dp</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dsa_switch * ds[4]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct dsa_device_ops *tag_ops</code>
</li>
<li>
<b>Field added. </b>
<code>enum dsa_tag_protocol default_proto</code>
</li>
<li>
<b>Field added. </b>
<code>struct net_device **lags</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int lags_len</code>
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
<code>unsigned int last_switch</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct net_device **lags</code> ➡️ <code>struct dsa_lag **lags</code>
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
