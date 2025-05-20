# Struct: <code>ethtool_phy_ops</code>

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
In <code>5.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ethtool_phy_ops {
    int (*get_sset_count)(struct phy_device *);
    int (*get_strings)(struct phy_device *, u8 *);
    int (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*start_cable_test)(struct phy_device *, struct netlink_ext_ack *);
    int (*start_cable_test_tdr)(struct phy_device *, struct netlink_ext_ack *, const struct phy_tdr_config *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ethtool_phy_ops {
    int (*get_sset_count)(struct phy_device *);
    int (*get_strings)(struct phy_device *, u8 *);
    int (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*start_cable_test)(struct phy_device *, struct netlink_ext_ack *);
    int (*start_cable_test_tdr)(struct phy_device *, struct netlink_ext_ack *, const struct phy_tdr_config *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ethtool_phy_ops {
    int (*get_sset_count)(struct phy_device *);
    int (*get_strings)(struct phy_device *, u8 *);
    int (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*start_cable_test)(struct phy_device *, struct netlink_ext_ack *);
    int (*start_cable_test_tdr)(struct phy_device *, struct netlink_ext_ack *, const struct phy_tdr_config *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ethtool_phy_ops {
    int (*get_sset_count)(struct phy_device *);
    int (*get_strings)(struct phy_device *, u8 *);
    int (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*start_cable_test)(struct phy_device *, struct netlink_ext_ack *);
    int (*start_cable_test_tdr)(struct phy_device *, struct netlink_ext_ack *, const struct phy_tdr_config *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ethtool_phy_ops {
    int (*get_sset_count)(struct phy_device *);
    int (*get_strings)(struct phy_device *, u8 *);
    int (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*start_cable_test)(struct phy_device *, struct netlink_ext_ack *);
    int (*start_cable_test_tdr)(struct phy_device *, struct netlink_ext_ack *, const struct phy_tdr_config *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ethtool_phy_ops {
    int (*get_sset_count)(struct phy_device *);
    int (*get_strings)(struct phy_device *, u8 *);
    int (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_plca_cfg)(struct phy_device *, struct phy_plca_cfg *);
    int (*set_plca_cfg)(struct phy_device *, const struct phy_plca_cfg *, struct netlink_ext_ack *);
    int (*get_plca_status)(struct phy_device *, struct phy_plca_status *);
    int (*start_cable_test)(struct phy_device *, struct netlink_ext_ack *);
    int (*start_cable_test_tdr)(struct phy_device *, struct netlink_ext_ack *, const struct phy_tdr_config *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ethtool_phy_ops {
    int (*get_sset_count)(struct phy_device *);
    int (*get_strings)(struct phy_device *, u8 *);
    int (*get_stats)(struct phy_device *, struct ethtool_stats *, u64 *);
    int (*get_plca_cfg)(struct phy_device *, struct phy_plca_cfg *);
    int (*set_plca_cfg)(struct phy_device *, const struct phy_plca_cfg *, struct netlink_ext_ack *);
    int (*get_plca_status)(struct phy_device *, struct phy_plca_status *);
    int (*start_cable_test)(struct phy_device *, struct netlink_ext_ack *);
    int (*start_cable_test_tdr)(struct phy_device *, struct netlink_ext_ack *, const struct phy_tdr_config *);
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*get_plca_cfg)(struct phy_device *, struct phy_plca_cfg *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_plca_cfg)(struct phy_device *, const struct phy_plca_cfg *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_plca_status)(struct phy_device *, struct phy_plca_status *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
