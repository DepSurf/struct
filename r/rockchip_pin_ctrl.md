# Struct: <code>rockchip_pin_ctrl</code>

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
struct rockchip_pin_ctrl {
    struct rockchip_pin_bank *pin_banks;
    u32 nr_banks;
    u32 nr_pins;
    char *label;
    enum rockchip_pinctrl_type type;
    int grf_mux_offset;
    int pmu_mux_offset;
    int grf_drv_offset;
    int pmu_drv_offset;
    struct rockchip_mux_recalced_data *iomux_recalced;
    u32 niomux_recalced;
    struct rockchip_mux_route_data *iomux_routes;
    u32 niomux_routes;
    void (*pull_calc_reg)(struct rockchip_pin_bank *, int, struct regmap **, int *, u8 *);
    void (*drv_calc_reg)(struct rockchip_pin_bank *, int, struct regmap **, int *, u8 *);
    int (*schmitt_calc_reg)(struct rockchip_pin_bank *, int, struct regmap **, int *, u8 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rockchip_pin_ctrl {
    struct rockchip_pin_bank *pin_banks;
    u32 nr_banks;
    u32 nr_pins;
    char *label;
    enum rockchip_pinctrl_type type;
    int grf_mux_offset;
    int pmu_mux_offset;
    int grf_drv_offset;
    int pmu_drv_offset;
    struct rockchip_mux_recalced_data *iomux_recalced;
    u32 niomux_recalced;
    struct rockchip_mux_route_data *iomux_routes;
    u32 niomux_routes;
    void (*pull_calc_reg)(struct rockchip_pin_bank *, int, struct regmap **, int *, u8 *);
    void (*drv_calc_reg)(struct rockchip_pin_bank *, int, struct regmap **, int *, u8 *);
    int (*schmitt_calc_reg)(struct rockchip_pin_bank *, int, struct regmap **, int *, u8 *);
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
