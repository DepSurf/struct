# Struct: <code>arizona</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
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
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct arizona {
    struct regmap *regmap;
    struct device *dev;
    enum arizona_type type;
    unsigned int rev;
    int num_core_supplies;
    struct regulator_bulk_data core_supplies[2];
    struct regulator *dcvdd;
    bool has_fully_powered_off;
    struct arizona_pdata pdata;
    unsigned int external_dcvdd;
    int irq;
    struct irq_domain *virq;
    struct regmap_irq_chip_data *aod_irq_chip;
    struct regmap_irq_chip_data *irq_chip;
    bool hpdet_clamp;
    unsigned int hp_ena;
    struct mutex clk_lock;
    int clk32k_ref;
    struct clk * mclk[2];
    bool ctrlif_error;
    struct snd_soc_dapm_context *dapm;
    int tdm_width[3];
    int tdm_slots[3];
    uint16_t dac_comp_coeff;
    uint8_t dac_comp_enabled;
    struct mutex dac_comp_lock;
    struct blocking_notifier_head notifier;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct blocking_notifier_head notifier</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct clk * mclk[2]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct snd_soc_dapm_context *dapm</code> ➡️ <code>struct snd_soc_dapm_context *dapm</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct clk * mclk[2]</code> ➡️ <code>struct clk * mclk[2]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
