# Struct: <code>ethtool_link_settings</code>

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
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u32 reserved[8];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u32 reserved[8];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u32 reserved[8];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 reserved1[1];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 reserved1[1];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 reserved1[1];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 reserved1[1];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 reserved1[1];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 rate_matching;
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 rate_matching;
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 master_slave_cfg;
    __u8 master_slave_state;
    __u8 rate_matching;
    __u32 reserved[7];
    __u32 link_mode_masks[0];
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
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
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
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ethtool_link_settings {
    __u32 cmd;
    __u32 speed;
    __u8 duplex;
    __u8 port;
    __u8 phy_address;
    __u8 autoneg;
    __u8 mdio_support;
    __u8 eth_tp_mdix;
    __u8 eth_tp_mdix_ctrl;
    __s8 link_mode_masks_nwords;
    __u8 transceiver;
    __u8 reserved1[3];
    __u32 reserved[7];
    __u32 link_mode_masks[0];
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 transceiver</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 reserved1[3]</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 reserved[8]</code> ➡️ <code>__u32 reserved[7]</code>
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
<code>__u8 master_slave_cfg</code>
</li>
<li>
<b>Field added. </b>
<code>__u8 master_slave_state</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u8 reserved1[3]</code> ➡️ <code>__u8 reserved1[1]</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 rate_matching</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 reserved1[1]</code>
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
