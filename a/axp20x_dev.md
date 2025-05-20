# Struct: <code>axp20x_dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    struct i2c_client *i2c_client;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct axp20x_dev {
    struct device *dev;
    int irq;
    long unsigned int irq_flags;
    struct regmap *regmap;
    struct regmap_irq_chip_data *regmap_irqc;
    long int variant;
    int nr_cells;
    const struct mfd_cell *cells;
    const struct regmap_config *regmap_cfg;
    const struct regmap_irq_chip *regmap_irq_chip;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
