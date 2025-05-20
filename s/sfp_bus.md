# Struct: <code>sfp_bus</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct net_device *netdev;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct net_device *netdev;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    const struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    const struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_quirk *sfp_quirk;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
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
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
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
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct sfp_bus {
    struct kref kref;
    struct list_head node;
    struct fwnode_handle *fwnode;
    const struct sfp_socket_ops *socket_ops;
    struct device *sfp_dev;
    struct sfp *sfp;
    const struct sfp_upstream_ops *upstream_ops;
    void *upstream;
    struct phy_device *phydev;
    bool registered;
    bool started;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct net_device *netdev</code>
</li>
</ul>
</details>
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
<code>const struct sfp_quirk *sfp_quirk</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct fwnode_handle *fwnode</code> ➡️ <code>const struct fwnode_handle *fwnode</code>
</li>
</ul>
</details>
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
