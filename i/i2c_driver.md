# Struct: <code>i2c_driver</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*attach_adapter)(struct i2c_adapter *);
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*attach_adapter)(struct i2c_adapter *);
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*attach_adapter)(struct i2c_adapter *);
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*attach_adapter)(struct i2c_adapter *);
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*attach_adapter)(struct i2c_adapter *);
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*attach_adapter)(struct i2c_adapter *);
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    void (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*remove)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    u32 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *);
    void (*remove)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    u32 flags;
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
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct i2c_driver {
    unsigned int class;
    int (*probe)(struct i2c_client *, const struct i2c_device_id *);
    int (*remove)(struct i2c_client *);
    int (*probe_new)(struct i2c_client *);
    void (*shutdown)(struct i2c_client *);
    void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int);
    int (*command)(struct i2c_client *, unsigned int, void *);
    struct device_driver driver;
    const struct i2c_device_id *id_table;
    int (*detect)(struct i2c_client *, struct i2c_board_info *);
    const short unsigned int *address_list;
    struct list_head clients;
    bool disable_i2c_core_irq_mapping;
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
<b>Field type changed. </b>
<code>void (*alert)(struct i2c_client *, unsigned int)</code> ➡️ <code>void (*alert)(struct i2c_client *, enum i2c_alert_protocol, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*probe_new)(struct i2c_client *)</code>
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
<code>bool disable_i2c_core_irq_mapping</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*attach_adapter)(struct i2c_adapter *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool disable_i2c_core_irq_mapping</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 flags</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*remove)(struct i2c_client *)</code> ➡️ <code>void (*remove)(struct i2c_client *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*probe)(struct i2c_client *, const struct i2c_device_id *)</code> ➡️ <code>int (*probe)(struct i2c_client *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*probe_new)(struct i2c_client *)</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
