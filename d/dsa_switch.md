# Struct: <code>dsa_switch</code>

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
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    int index;
    void *priv;
    struct dsa_chip_data *cd;
    struct dsa_switch_driver *drv;
    s8 rtable[4];
    char hwmon_name[24];
    struct device *hwmon_dev;
    struct net_device *master_netdev;
    u32 dsa_port_mask;
    u32 cpu_port_mask;
    u32 enabled_port_mask;
    u32 phys_mii_mask;
    struct dsa_port ports[12];
    struct mii_bus *slave_mii_bus;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    int index;
    void *priv;
    struct dsa_chip_data *cd;
    struct dsa_switch_ops *ops;
    s8 rtable[4];
    char hwmon_name[24];
    struct device *hwmon_dev;
    struct net_device *master_netdev;
    u32 dsa_port_mask;
    u32 cpu_port_mask;
    u32 enabled_port_mask;
    u32 phys_mii_mask;
    struct dsa_port ports[12];
    struct mii_bus *slave_mii_bus;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 dsa_port_mask;
    u32 cpu_port_mask;
    u32 enabled_port_mask;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    long unsigned int *bitmap;
    long unsigned int _bitmap;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    long unsigned int *bitmap;
    long unsigned int _bitmap;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dsa_switch {
    bool setup;
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool configure_vlan_while_not_filtering;
    bool vlan_filtering;
    bool pcs_poll;
    bool mtu_enforcement_ingress;
    size_t num_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dsa_switch {
    bool setup;
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool configure_vlan_while_not_filtering;
    bool untag_bridge_pvid;
    bool vlan_filtering;
    bool pcs_poll;
    bool mtu_enforcement_ingress;
    size_t num_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dsa_switch {
    bool setup;
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool configure_vlan_while_not_filtering;
    bool untag_bridge_pvid;
    bool assisted_learning_on_cpu_port;
    bool vlan_filtering;
    bool pcs_poll;
    bool mtu_enforcement_ingress;
    unsigned int num_lag_ids;
    size_t num_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dsa_switch {
    bool setup;
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct dsa_8021q_context *tag_8021q_ctx;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool needs_standalone_vlan_filtering;
    bool configure_vlan_while_not_filtering;
    bool untag_bridge_pvid;
    bool assisted_learning_on_cpu_port;
    bool vlan_filtering;
    bool pcs_poll;
    bool mtu_enforcement_ingress;
    unsigned int num_lag_ids;
    unsigned int num_fwd_offloading_bridges;
    size_t num_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    u32 setup;
    u32 vlan_filtering_is_global;
    u32 needs_standalone_vlan_filtering;
    u32 configure_vlan_while_not_filtering;
    u32 untag_bridge_pvid;
    u32 assisted_learning_on_cpu_port;
    u32 vlan_filtering;
    u32 mtu_enforcement_ingress;
    u32 fdb_isolation;
    struct notifier_block nb;
    void *priv;
    void *tagger_data;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct dsa_8021q_context *tag_8021q_ctx;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    unsigned int num_lag_ids;
    unsigned int max_num_bridges;
    unsigned int num_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    u32 setup;
    u32 vlan_filtering_is_global;
    u32 needs_standalone_vlan_filtering;
    u32 configure_vlan_while_not_filtering;
    u32 untag_bridge_pvid;
    u32 assisted_learning_on_cpu_port;
    u32 vlan_filtering;
    u32 mtu_enforcement_ingress;
    u32 fdb_isolation;
    struct notifier_block nb;
    void *priv;
    void *tagger_data;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct dsa_8021q_context *tag_8021q_ctx;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    unsigned int num_lag_ids;
    unsigned int max_num_bridges;
    unsigned int num_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    u32 setup;
    u32 vlan_filtering_is_global;
    u32 needs_standalone_vlan_filtering;
    u32 configure_vlan_while_not_filtering;
    u32 untag_bridge_pvid;
    u32 assisted_learning_on_cpu_port;
    u32 vlan_filtering;
    u32 mtu_enforcement_ingress;
    u32 fdb_isolation;
    struct notifier_block nb;
    void *priv;
    void *tagger_data;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct dsa_8021q_context *tag_8021q_ctx;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    unsigned int num_lag_ids;
    unsigned int max_num_bridges;
    unsigned int num_ports;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    u32 setup;
    u32 vlan_filtering_is_global;
    u32 needs_standalone_vlan_filtering;
    u32 configure_vlan_while_not_filtering;
    u32 untag_bridge_pvid;
    u32 assisted_learning_on_cpu_port;
    u32 vlan_filtering;
    u32 mtu_enforcement_ingress;
    u32 fdb_isolation;
    struct notifier_block nb;
    void *priv;
    void *tagger_data;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    u32 phys_mii_mask;
    struct mii_bus *user_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct dsa_8021q_context *tag_8021q_ctx;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    unsigned int num_lag_ids;
    unsigned int max_num_bridges;
    unsigned int num_ports;
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
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
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
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dsa_switch {
    struct device *dev;
    struct dsa_switch_tree *dst;
    unsigned int index;
    struct notifier_block nb;
    void *priv;
    struct dsa_chip_data *cd;
    const struct dsa_switch_ops *ops;
    s8 rtable[4];
    u32 phys_mii_mask;
    struct mii_bus *slave_mii_bus;
    unsigned int ageing_time_min;
    unsigned int ageing_time_max;
    struct devlink *devlink;
    unsigned int num_tx_queues;
    bool vlan_filtering_is_global;
    bool vlan_filtering;
    size_t num_ports;
    struct dsa_port ports[0];
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
<code>struct dsa_switch_ops *ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dsa_switch_driver *drv</code>
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
<code>struct notifier_block nb</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ageing_time_min</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ageing_time_max</code>
</li>
<li>
<b>Field added. </b>
<code>struct devlink *devlink</code>
</li>
<li>
<b>Field added. </b>
<code>size_t num_ports</code>
</li>
<li>
<b>Field removed. </b>
<code>char hwmon_name[24]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *hwmon_dev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct net_device *master_netdev</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dsa_switch_ops *ops</code> ➡️ <code>const struct dsa_switch_ops *ops</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct dsa_port ports[12]</code> ➡️ <code>struct dsa_port ports[0]</code>
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
<code>unsigned int num_tx_queues</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 dsa_port_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 cpu_port_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 enabled_port_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>int index</code> ➡️ <code>unsigned int index</code>
</li>
</ul>
</details>
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
<code>long unsigned int *bitmap</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int _bitmap</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool vlan_filtering_is_global</code>
</li>
<li>
<b>Field added. </b>
<code>bool vlan_filtering</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int *bitmap</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int _bitmap</code>
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
<code>bool setup</code>
</li>
<li>
<b>Field added. </b>
<code>bool configure_vlan_while_not_filtering</code>
</li>
<li>
<b>Field added. </b>
<code>bool pcs_poll</code>
</li>
<li>
<b>Field added. </b>
<code>bool mtu_enforcement_ingress</code>
</li>
<li>
<b>Field removed. </b>
<code>s8 rtable[4]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct dsa_port ports[0]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool untag_bridge_pvid</code>
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
<code>bool assisted_learning_on_cpu_port</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int num_lag_ids</code>
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
<code>struct dsa_8021q_context *tag_8021q_ctx</code>
</li>
<li>
<b>Field added. </b>
<code>bool needs_standalone_vlan_filtering</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int num_fwd_offloading_bridges</code>
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
<code>u32 fdb_isolation</code>
</li>
<li>
<b>Field added. </b>
<code>void *tagger_data</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int max_num_bridges</code>
</li>
<li>
<b>Field removed. </b>
<code>bool pcs_poll</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int num_fwd_offloading_bridges</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool setup</code> ➡️ <code>u32 setup</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool vlan_filtering_is_global</code> ➡️ <code>u32 vlan_filtering_is_global</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool needs_standalone_vlan_filtering</code> ➡️ <code>u32 needs_standalone_vlan_filtering</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool configure_vlan_while_not_filtering</code> ➡️ <code>u32 configure_vlan_while_not_filtering</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool untag_bridge_pvid</code> ➡️ <code>u32 untag_bridge_pvid</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool assisted_learning_on_cpu_port</code> ➡️ <code>u32 assisted_learning_on_cpu_port</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool vlan_filtering</code> ➡️ <code>u32 vlan_filtering</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool mtu_enforcement_ingress</code> ➡️ <code>u32 mtu_enforcement_ingress</code>
</li>
<li>
<b>Field type changed. </b>
<code>size_t num_ports</code> ➡️ <code>unsigned int num_ports</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mii_bus *user_mii_bus</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mii_bus *slave_mii_bus</code>
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
