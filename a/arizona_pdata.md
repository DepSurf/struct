# Struct: <code>arizona_pdata</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct arizona_pdata {
    int reset;
    int ldoena;
    struct regulator_init_data *micvdd;
    struct regulator_init_data *ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    bool out_mono[6];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct arizona_pdata {
    int reset;
    int ldoena;
    struct regulator_init_data *micvdd;
    struct regulator_init_data *ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct arizona_pdata {
    int reset;
    int ldoena;
    struct regulator_init_data *micvdd;
    struct regulator_init_data *ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct arizona_pdata {
    int reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct arizona_pdata {
    int reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
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
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
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
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct arizona_pdata {
    struct gpio_desc *reset;
    struct arizona_micsupp_pdata micvdd;
    struct arizona_ldo1_pdata ldo1;
    int clk32k_src;
    unsigned int irq_flags;
    int gpio_base;
    unsigned int gpio_defaults[5];
    unsigned int max_channels_clocked[3];
    bool jd_gpio5;
    bool jd_gpio5_nopull;
    bool jd_invert;
    bool hpdet_acc_id;
    bool hpdet_acc_id_line;
    int hpdet_id_gpio;
    unsigned int hpdet_channel;
    bool micd_software_compare;
    unsigned int micd_detect_debounce;
    int micd_pol_gpio;
    unsigned int micd_bias_start_time;
    unsigned int micd_rate;
    unsigned int micd_dbtime;
    unsigned int micd_timeout;
    bool micd_force_micbias;
    const struct arizona_micd_range *micd_ranges;
    int num_micd_ranges;
    struct arizona_micd_config *micd_configs;
    int num_micd_configs;
    int dmic_ref[4];
    struct arizona_micbias micbias[3];
    int inmode[4];
    int out_mono[6];
    unsigned int out_vol_limit[12];
    unsigned int spk_mute[2];
    unsigned int spk_fmt[2];
    unsigned int hap_act;
    int irq_gpio;
    unsigned int gpsw;
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
<b>Field type changed. </b>
<code>bool out_mono[6]</code> ➡️ <code>int out_mono[6]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int ldoena</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct regulator_init_data *micvdd</code> ➡️ <code>struct arizona_micsupp_pdata micvdd</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct regulator_init_data *ldo1</code> ➡️ <code>struct arizona_ldo1_pdata ldo1</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int out_vol_limit[12]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int reset</code> ➡️ <code>struct gpio_desc *reset</code>
</li>
</ul>
</details>
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
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
