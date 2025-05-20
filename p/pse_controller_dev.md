# Struct: <code>pse_controller_dev</code>

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
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pse_controller_dev {
    const struct pse_controller_ops *ops;
    struct module *owner;
    struct list_head list;
    struct list_head pse_control_head;
    struct device *dev;
    int of_pse_n_cells;
    int (*of_xlate)(struct pse_controller_dev *, const struct of_phandle_args *);
    unsigned int nr_lines;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pse_controller_dev {
    const struct pse_controller_ops *ops;
    struct module *owner;
    struct list_head list;
    struct list_head pse_control_head;
    struct device *dev;
    int of_pse_n_cells;
    int (*of_xlate)(struct pse_controller_dev *, const struct of_phandle_args *);
    unsigned int nr_lines;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pse_controller_dev {
    const struct pse_controller_ops *ops;
    struct module *owner;
    struct list_head list;
    struct list_head pse_control_head;
    struct device *dev;
    int of_pse_n_cells;
    int (*of_xlate)(struct pse_controller_dev *, const struct of_phandle_args *);
    unsigned int nr_lines;
    struct mutex lock;
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
