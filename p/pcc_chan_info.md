# Struct: <code>pcc_chan_info</code>

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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pcc_chan_info {
    struct pcc_mbox_chan chan;
    struct pcc_chan_reg db;
    struct pcc_chan_reg plat_irq_ack;
    struct pcc_chan_reg cmd_complete;
    struct pcc_chan_reg cmd_update;
    struct pcc_chan_reg error;
    int plat_irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pcc_chan_info {
    struct pcc_mbox_chan chan;
    struct pcc_chan_reg db;
    struct pcc_chan_reg plat_irq_ack;
    struct pcc_chan_reg cmd_complete;
    struct pcc_chan_reg cmd_update;
    struct pcc_chan_reg error;
    int plat_irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pcc_chan_info {
    struct pcc_mbox_chan chan;
    struct pcc_chan_reg db;
    struct pcc_chan_reg plat_irq_ack;
    struct pcc_chan_reg cmd_complete;
    struct pcc_chan_reg cmd_update;
    struct pcc_chan_reg error;
    int plat_irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pcc_chan_info {
    struct pcc_mbox_chan chan;
    struct pcc_chan_reg db;
    struct pcc_chan_reg plat_irq_ack;
    struct pcc_chan_reg cmd_complete;
    struct pcc_chan_reg cmd_update;
    struct pcc_chan_reg error;
    int plat_irq;
    u8 type;
    unsigned int plat_irq_flags;
    bool chan_in_use;
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
<code>u8 type</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int plat_irq_flags</code>
</li>
<li>
<b>Field added. </b>
<code>bool chan_in_use</code>
</li>
</ul>
</details>
</li>
</ul>
