# Struct: <code>omap_i2c_dev</code>

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
struct omap_i2c_dev {
    struct device *dev;
    void *base;
    int irq;
    int reg_shift;
    struct completion cmd_complete;
    struct resource *ioarea;
    u32 latency;
    void (*set_mpu_wkup_lat)(struct device *, long int);
    u32 speed;
    u32 flags;
    u16 scheme;
    u16 cmd_err;
    u8 *buf;
    u8 *regs;
    size_t buf_len;
    struct i2c_adapter adapter;
    u8 threshold;
    u8 fifo_size;
    u32 rev;
    unsigned int b_hw;
    unsigned int bb_valid;
    unsigned int receiver;
    u16 iestate;
    u16 pscstate;
    u16 scllstate;
    u16 sclhstate;
    u16 syscstate;
    u16 westate;
    u16 errata;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct omap_i2c_dev {
    struct device *dev;
    void *base;
    int irq;
    int reg_shift;
    struct completion cmd_complete;
    struct resource *ioarea;
    u32 latency;
    void (*set_mpu_wkup_lat)(struct device *, long int);
    u32 speed;
    u32 flags;
    u16 scheme;
    u16 cmd_err;
    u8 *buf;
    u8 *regs;
    size_t buf_len;
    struct i2c_adapter adapter;
    u8 threshold;
    u8 fifo_size;
    u32 rev;
    unsigned int b_hw;
    unsigned int bb_valid;
    unsigned int receiver;
    u16 iestate;
    u16 pscstate;
    u16 scllstate;
    u16 sclhstate;
    u16 syscstate;
    u16 westate;
    u16 errata;
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
