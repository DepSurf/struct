# Struct: <code>pcs_device</code>

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
struct pcs_device {
    struct resource *res;
    void *base;
    void *saved_vals;
    unsigned int size;
    struct device *dev;
    struct device_node *np;
    struct pinctrl_dev *pctl;
    unsigned int flags;
    struct property *missing_nr_pinctrl_cells;
    struct pcs_soc_data socdata;
    raw_spinlock_t lock;
    struct mutex mutex;
    unsigned int width;
    unsigned int fmask;
    unsigned int fshift;
    unsigned int foff;
    unsigned int fmax;
    bool bits_per_mux;
    unsigned int bits_per_pin;
    struct pcs_data pins;
    struct list_head gpiofuncs;
    struct list_head irqs;
    struct irq_chip chip;
    struct irq_domain *domain;
    struct pinctrl_desc desc;
    unsigned int (*read)(void *);
    void (*write)(unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pcs_device {
    struct resource *res;
    void *base;
    void *saved_vals;
    unsigned int size;
    struct device *dev;
    struct device_node *np;
    struct pinctrl_dev *pctl;
    unsigned int flags;
    struct property *missing_nr_pinctrl_cells;
    struct pcs_soc_data socdata;
    raw_spinlock_t lock;
    struct mutex mutex;
    unsigned int width;
    unsigned int fmask;
    unsigned int fshift;
    unsigned int foff;
    unsigned int fmax;
    bool bits_per_mux;
    unsigned int bits_per_pin;
    struct pcs_data pins;
    struct list_head gpiofuncs;
    struct list_head irqs;
    struct irq_chip chip;
    struct irq_domain *domain;
    struct pinctrl_desc desc;
    unsigned int (*read)(void *);
    void (*write)(unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pcs_device {
    struct resource *res;
    void *base;
    void *saved_vals;
    unsigned int size;
    struct device *dev;
    struct device_node *np;
    struct pinctrl_dev *pctl;
    unsigned int flags;
    struct property *missing_nr_pinctrl_cells;
    struct pcs_soc_data socdata;
    raw_spinlock_t lock;
    struct mutex mutex;
    unsigned int width;
    unsigned int fmask;
    unsigned int fshift;
    unsigned int foff;
    unsigned int fmax;
    bool bits_per_mux;
    unsigned int bits_per_pin;
    struct pcs_data pins;
    struct list_head gpiofuncs;
    struct list_head irqs;
    struct irq_chip chip;
    struct irq_domain *domain;
    struct pinctrl_desc desc;
    unsigned int (*read)(void *);
    void (*write)(unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pcs_device {
    struct resource *res;
    void *base;
    void *saved_vals;
    unsigned int size;
    struct device *dev;
    struct device_node *np;
    struct pinctrl_dev *pctl;
    unsigned int flags;
    struct property *missing_nr_pinctrl_cells;
    struct pcs_soc_data socdata;
    raw_spinlock_t lock;
    struct mutex mutex;
    unsigned int width;
    unsigned int fmask;
    unsigned int fshift;
    unsigned int foff;
    unsigned int fmax;
    bool bits_per_mux;
    unsigned int bits_per_pin;
    struct pcs_data pins;
    struct list_head gpiofuncs;
    struct list_head irqs;
    struct irq_chip chip;
    struct irq_domain *domain;
    struct pinctrl_desc desc;
    unsigned int (*read)(void *);
    void (*write)(unsigned int, void *);
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
