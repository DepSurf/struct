# Struct: <code>intel_soc_pmic</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_level2;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_level2;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_level2;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
    enum intel_cht_wc_models cht_wc_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
    enum intel_cht_wc_models cht_wc_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
    enum intel_cht_wc_models cht_wc_model;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
    struct intel_scu_ipc_dev *scu;
    enum intel_cht_wc_models cht_wc_model;
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct intel_soc_pmic {
    int irq;
    struct regmap *regmap;
    struct regmap_irq_chip_data *irq_chip_data;
    struct regmap_irq_chip_data *irq_chip_data_pwrbtn;
    struct regmap_irq_chip_data *irq_chip_data_tmu;
    struct regmap_irq_chip_data *irq_chip_data_bcu;
    struct regmap_irq_chip_data *irq_chip_data_adc;
    struct regmap_irq_chip_data *irq_chip_data_chgr;
    struct regmap_irq_chip_data *irq_chip_data_crit;
    struct device *dev;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct regmap_irq_chip_data *irq_chip_data_tmu</code>
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
<code>struct regmap_irq_chip_data *irq_chip_data_bcu</code>
</li>
<li>
<b>Field added. </b>
<code>struct regmap_irq_chip_data *irq_chip_data_adc</code>
</li>
<li>
<b>Field added. </b>
<code>struct regmap_irq_chip_data *irq_chip_data_chgr</code>
</li>
<li>
<b>Field added. </b>
<code>struct regmap_irq_chip_data *irq_chip_data_crit</code>
</li>
<li>
<b>Field removed. </b>
<code>struct regmap_irq_chip_data *irq_chip_data_level2</code>
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
<b>Field added. </b>
<code>struct regmap_irq_chip_data *irq_chip_data_pwrbtn</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct intel_scu_ipc_dev *scu</code>
</li>
</ul>
</details>
</li>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum intel_cht_wc_models cht_wc_model</code>
</li>
</ul>
</details>
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
<b>Arch</b>
<ul>
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
