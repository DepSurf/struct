# Struct: <code>ahci_port_priv</code>

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
struct ahci_port_priv {
    struct ata_link *active_link;
    struct ahci_cmd_hdr *cmd_slot;
    dma_addr_t cmd_slot_dma;
    void *cmd_tbl;
    dma_addr_t cmd_tbl_dma;
    void *rx_fis;
    dma_addr_t rx_fis_dma;
    unsigned int ncq_saw_d2h;
    unsigned int ncq_saw_dmas;
    unsigned int ncq_saw_sdb;
    spinlock_t lock;
    u32 intr_mask;
    bool fbs_supported;
    bool fbs_enabled;
    int fbs_last_dev;
    struct ahci_em_priv em_priv[8];
    char *irq_desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ahci_port_priv {
    struct ata_link *active_link;
    struct ahci_cmd_hdr *cmd_slot;
    dma_addr_t cmd_slot_dma;
    void *cmd_tbl;
    dma_addr_t cmd_tbl_dma;
    void *rx_fis;
    dma_addr_t rx_fis_dma;
    unsigned int ncq_saw_d2h;
    unsigned int ncq_saw_dmas;
    unsigned int ncq_saw_sdb;
    spinlock_t lock;
    u32 intr_mask;
    bool fbs_supported;
    bool fbs_enabled;
    int fbs_last_dev;
    struct ahci_em_priv em_priv[8];
    char *irq_desc;
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
