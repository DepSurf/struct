# Struct: <code>cec_pin_ops</code>

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
struct cec_pin_ops {
    bool (*read)(struct cec_adapter *);
    void (*low)(struct cec_adapter *);
    void (*high)(struct cec_adapter *);
    bool (*enable_irq)(struct cec_adapter *);
    void (*disable_irq)(struct cec_adapter *);
    void (*free)(struct cec_adapter *);
    void (*status)(struct cec_adapter *, struct seq_file *);
    int (*read_hpd)(struct cec_adapter *);
    int (*read_5v)(struct cec_adapter *);
};
```
</details>
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
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cec_pin_ops {
    bool (*read)(struct cec_adapter *);
    void (*low)(struct cec_adapter *);
    void (*high)(struct cec_adapter *);
    bool (*enable_irq)(struct cec_adapter *);
    void (*disable_irq)(struct cec_adapter *);
    void (*free)(struct cec_adapter *);
    void (*status)(struct cec_adapter *, struct seq_file *);
    int (*read_hpd)(struct cec_adapter *);
    int (*read_5v)(struct cec_adapter *);
};
```
</details>
</li>
</ul>

## Differences
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
</ul>
