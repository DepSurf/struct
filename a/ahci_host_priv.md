# Struct: <code>ahci_host_priv</code>

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
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct ahci_host_priv {
    unsigned int flags;
    u32 force_port_map;
    u32 mask_port_map;
    void *mmio;
    u32 cap;
    u32 cap2;
    u32 version;
    u32 port_map;
    u32 saved_cap;
    u32 saved_cap2;
    u32 saved_port_map;
    u32 em_loc;
    u32 em_buf_sz;
    u32 em_msg_type;
    u32 remapped_nvme;
    bool got_runtime_pm;
    struct clk * clks[5];
    struct reset_control *rsts;
    struct regulator **target_pwrs;
    struct regulator *ahci_regulator;
    struct regulator *phy_regulator;
    struct phy **phys;
    unsigned int nports;
    void *plat_data;
    unsigned int irq;
    void (*start_engine)(struct ata_port *);
    int (*stop_engine)(struct ata_port *);
    irqreturn_t (*irq_handler)(int, void *);
    int (*get_irq_vector)(struct ata_host *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ahci_host_priv {
    unsigned int flags;
    u32 force_port_map;
    u32 mask_port_map;
    void *mmio;
    u32 cap;
    u32 cap2;
    u32 version;
    u32 port_map;
    u32 saved_cap;
    u32 saved_cap2;
    u32 saved_port_map;
    u32 em_loc;
    u32 em_buf_sz;
    u32 em_msg_type;
    u32 remapped_nvme;
    bool got_runtime_pm;
    struct clk * clks[5];
    struct reset_control *rsts;
    struct regulator **target_pwrs;
    struct regulator *ahci_regulator;
    struct regulator *phy_regulator;
    struct phy **phys;
    unsigned int nports;
    void *plat_data;
    unsigned int irq;
    void (*start_engine)(struct ata_port *);
    int (*stop_engine)(struct ata_port *);
    irqreturn_t (*irq_handler)(int, void *);
    int (*get_irq_vector)(struct ata_host *, int);
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
