# Struct: <code>si_sm_io</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct si_sm_io {
    unsigned char (*inputb)(const struct si_sm_io *, unsigned int);
    void (*outputb)(const struct si_sm_io *, unsigned int, unsigned char);
    void *addr;
    int regspacing;
    int regsize;
    int regshift;
    int addr_type;
    long int addr_data;
    enum ipmi_addr_src addr_source;
    void (*addr_source_cleanup)(struct si_sm_io *);
    void *addr_source_data;
    union ipmi_smi_info_union addr_info;
    int (*io_setup)(struct si_sm_io *);
    void (*io_cleanup)(struct si_sm_io *);
    unsigned int io_size;
    int irq;
    int (*irq_setup)(struct si_sm_io *);
    void *irq_handler_data;
    void (*irq_cleanup)(struct si_sm_io *);
    u8 slave_addr;
    enum si_type si_type;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct si_sm_io {
    unsigned char (*inputb)(const struct si_sm_io *, unsigned int);
    void (*outputb)(const struct si_sm_io *, unsigned int, unsigned char);
    void *addr;
    int regspacing;
    int regsize;
    int regshift;
    int addr_type;
    long int addr_data;
    enum ipmi_addr_src addr_source;
    void (*addr_source_cleanup)(struct si_sm_io *);
    void *addr_source_data;
    union ipmi_smi_info_union addr_info;
    int (*io_setup)(struct si_sm_io *);
    void (*io_cleanup)(struct si_sm_io *);
    unsigned int io_size;
    int irq;
    int (*irq_setup)(struct si_sm_io *);
    void *irq_handler_data;
    void (*irq_cleanup)(struct si_sm_io *);
    u8 slave_addr;
    enum si_type si_type;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct si_sm_io {
    unsigned char (*inputb)(const struct si_sm_io *, unsigned int);
    void (*outputb)(const struct si_sm_io *, unsigned int, unsigned char);
    void *addr;
    int regspacing;
    int regsize;
    int regshift;
    int addr_type;
    long int addr_data;
    enum ipmi_addr_src addr_source;
    void (*addr_source_cleanup)(struct si_sm_io *);
    void *addr_source_data;
    union ipmi_smi_info_union addr_info;
    int (*io_setup)(struct si_sm_io *);
    void (*io_cleanup)(struct si_sm_io *);
    unsigned int io_size;
    int irq;
    int (*irq_setup)(struct si_sm_io *);
    void *irq_handler_data;
    void (*irq_cleanup)(struct si_sm_io *);
    u8 slave_addr;
    enum si_type si_type;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct si_sm_io {
    unsigned char (*inputb)(const struct si_sm_io *, unsigned int);
    void (*outputb)(const struct si_sm_io *, unsigned int, unsigned char);
    void *addr;
    unsigned int regspacing;
    unsigned int regsize;
    unsigned int regshift;
    enum ipmi_addr_space addr_space;
    long unsigned int addr_data;
    enum ipmi_addr_src addr_source;
    void (*addr_source_cleanup)(struct si_sm_io *);
    void *addr_source_data;
    union ipmi_smi_info_union addr_info;
    int (*io_setup)(struct si_sm_io *);
    void (*io_cleanup)(struct si_sm_io *);
    unsigned int io_size;
    int irq;
    int (*irq_setup)(struct si_sm_io *);
    void *irq_handler_data;
    void (*irq_cleanup)(struct si_sm_io *);
    u8 slave_addr;
    enum si_type si_type;
    struct device *dev;
};
```
</details>
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum ipmi_addr_space addr_space</code>
</li>
<li>
<b>Field removed. </b>
<code>int addr_type</code>
</li>
<li>
<b>Field type changed. </b>
<code>int regspacing</code> ➡️ <code>unsigned int regspacing</code>
</li>
<li>
<b>Field type changed. </b>
<code>int regsize</code> ➡️ <code>unsigned int regsize</code>
</li>
<li>
<b>Field type changed. </b>
<code>int regshift</code> ➡️ <code>unsigned int regshift</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int addr_data</code> ➡️ <code>long unsigned int addr_data</code>
</li>
</ul>
</details>
</li>
</ul>
