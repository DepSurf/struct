# Struct: <code>mii_bus</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[17];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct phy_device * phy_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int *irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[17];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[17];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    unsigned int is_managed;
    unsigned int is_managed_registered;
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    int reset_post_delay_us;
    struct gpio_desc *reset_gpiod;
    enum (anon) probe_capabilities;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    int reset_post_delay_us;
    struct gpio_desc *reset_gpiod;
    enum (anon) probe_capabilities;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    int reset_post_delay_us;
    struct gpio_desc *reset_gpiod;
    enum (anon) probe_capabilities;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    int reset_post_delay_us;
    struct gpio_desc *reset_gpiod;
    enum (anon) probe_capabilities;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    int reset_post_delay_us;
    struct gpio_desc *reset_gpiod;
    enum (anon) probe_capabilities;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*read_c45)(struct mii_bus *, int, int, int);
    int (*write_c45)(struct mii_bus *, int, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    int reset_post_delay_us;
    struct gpio_desc *reset_gpiod;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*read_c45)(struct mii_bus *, int, int, int);
    int (*write_c45)(struct mii_bus *, int, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mdio_bus_stats stats[32];
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    int reset_post_delay_us;
    struct gpio_desc *reset_gpiod;
    struct mutex shared_lock;
    struct phy_package_shared * shared[32];
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
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
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
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mii_bus {
    struct module *owner;
    const char *name;
    char id[61];
    void *priv;
    int (*read)(struct mii_bus *, int, int);
    int (*write)(struct mii_bus *, int, int, u16);
    int (*reset)(struct mii_bus *);
    struct mutex mdio_lock;
    struct device *parent;
    enum (anon) state;
    struct device dev;
    struct mdio_device * mdio_map[32];
    u32 phy_mask;
    u32 phy_ignore_ta_mask;
    int irq[32];
    int reset_delay_us;
    struct gpio_desc *reset_gpiod;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mdio_device * mdio_map[32]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct phy_device * phy_map[32]</code>
</li>
<li>
<b>Field type changed. </b>
<code>int *irq</code> ➡️ <code>int irq[32]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int reset_delay_us</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_desc *reset_gpiod</code>
</li>
<li>
<b>Field type changed. </b>
<code>char id[17]</code> ➡️ <code>char id[61]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mdio_bus_stats stats[32]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int is_managed</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int is_managed_registered</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex shared_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct phy_package_shared * shared[32]</code>
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
<code>int reset_post_delay_us</code>
</li>
<li>
<b>Field added. </b>
<code>enum (anon) probe_capabilities</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int is_managed</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int is_managed_registered</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>int (*read_c45)(struct mii_bus *, int, int, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*write_c45)(struct mii_bus *, int, int, int, u16)</code>
</li>
<li>
<b>Field removed. </b>
<code>enum (anon) probe_capabilities</code>
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
