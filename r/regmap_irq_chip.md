# Struct: <code>regmap_irq_chip</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int irq_reg_stride;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool clear_ack;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int *virt_reg_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool clear_ack;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    bool not_fixed_stride;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    int num_virt_regs;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    int (*set_type_virt)(unsigned int **, unsigned int, long unsigned int, int);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int *virt_reg_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool clear_ack;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    bool not_fixed_stride;
    bool status_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    int num_virt_regs;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    int (*set_type_virt)(unsigned int **, unsigned int, long unsigned int, int);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int *virt_reg_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool clear_ack;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    bool not_fixed_stride;
    bool status_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    int num_virt_regs;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    int (*set_type_virt)(unsigned int **, unsigned int, long unsigned int, int);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int *virt_reg_base;
    const unsigned int *config_base;
    unsigned int irq_reg_stride;
    unsigned int init_ack_masked;
    unsigned int mask_invert;
    unsigned int mask_unmask_non_inverted;
    unsigned int use_ack;
    unsigned int ack_invert;
    unsigned int clear_ack;
    unsigned int wake_invert;
    unsigned int runtime_pm;
    unsigned int type_invert;
    unsigned int type_in_mask;
    unsigned int clear_on_unmask;
    unsigned int not_fixed_stride;
    unsigned int status_invert;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    int num_virt_regs;
    int num_config_bases;
    int num_config_regs;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    int (*handle_mask_sync)(struct regmap *, int, unsigned int, unsigned int, void *);
    int (*set_type_virt)(unsigned int **, unsigned int, long unsigned int, int);
    int (*set_type_config)(unsigned int **, unsigned int, const struct regmap_irq *, int);
    unsigned int (*get_irq_reg)(struct regmap_irq_chip_data *, unsigned int, int);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    const unsigned int *config_base;
    unsigned int irq_reg_stride;
    unsigned int init_ack_masked;
    unsigned int mask_unmask_non_inverted;
    unsigned int use_ack;
    unsigned int ack_invert;
    unsigned int clear_ack;
    unsigned int status_invert;
    unsigned int wake_invert;
    unsigned int type_in_mask;
    unsigned int clear_on_unmask;
    unsigned int runtime_pm;
    unsigned int no_status;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_config_bases;
    int num_config_regs;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    int (*handle_mask_sync)(int, unsigned int, unsigned int, void *);
    int (*set_type_config)(unsigned int **, unsigned int, const struct regmap_irq *, int, void *);
    unsigned int (*get_irq_reg)(struct regmap_irq_chip_data *, unsigned int, int);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    const unsigned int *config_base;
    unsigned int irq_reg_stride;
    unsigned int init_ack_masked;
    unsigned int mask_unmask_non_inverted;
    unsigned int use_ack;
    unsigned int ack_invert;
    unsigned int clear_ack;
    unsigned int status_invert;
    unsigned int wake_invert;
    unsigned int type_in_mask;
    unsigned int clear_on_unmask;
    unsigned int runtime_pm;
    unsigned int no_status;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_config_bases;
    int num_config_regs;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    int (*handle_mask_sync)(int, unsigned int, unsigned int, void *);
    int (*set_type_config)(unsigned int **, unsigned int, const struct regmap_irq *, int, void *);
    unsigned int (*get_irq_reg)(struct regmap_irq_chip_data *, unsigned int, int);
    void *irq_drv_data;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
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
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct regmap_irq_chip {
    const char *name;
    unsigned int main_status;
    unsigned int num_main_status_bits;
    struct regmap_irq_sub_irq_map *sub_reg_offsets;
    int num_main_regs;
    unsigned int status_base;
    unsigned int mask_base;
    unsigned int unmask_base;
    unsigned int ack_base;
    unsigned int wake_base;
    unsigned int type_base;
    unsigned int irq_reg_stride;
    bool mask_writeonly;
    bool init_ack_masked;
    bool mask_invert;
    bool use_ack;
    bool ack_invert;
    bool wake_invert;
    bool runtime_pm;
    bool type_invert;
    bool type_in_mask;
    bool clear_on_unmask;
    int num_regs;
    const struct regmap_irq *irqs;
    int num_irqs;
    int num_type_reg;
    unsigned int type_reg_stride;
    int (*handle_pre_irq)(void *);
    int (*handle_post_irq)(void *);
    void *irq_drv_data;
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
<code>unsigned int type_base</code>
</li>
<li>
<b>Field added. </b>
<code>bool type_invert</code>
</li>
<li>
<b>Field added. </b>
<code>int num_type_reg</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int type_reg_stride</code>
</li>
<li>
<b>Field added. </b>
<code>int (*handle_pre_irq)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*handle_post_irq)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void *irq_drv_data</code>
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
<b>Field added. </b>
<code>bool mask_writeonly</code>
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
<code>bool type_in_mask</code>
</li>
<li>
<b>Field added. </b>
<code>bool clear_on_unmask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int main_status</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int num_main_status_bits</code>
</li>
<li>
<b>Field added. </b>
<code>struct regmap_irq_sub_irq_map *sub_reg_offsets</code>
</li>
<li>
<b>Field added. </b>
<code>int num_main_regs</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool clear_ack</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int *virt_reg_base</code>
</li>
<li>
<b>Field added. </b>
<code>bool not_fixed_stride</code>
</li>
<li>
<b>Field added. </b>
<code>int num_virt_regs</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_type_virt)(unsigned int **, unsigned int, long unsigned int, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool status_invert</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const unsigned int *config_base</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int mask_unmask_non_inverted</code>
</li>
<li>
<b>Field added. </b>
<code>int num_config_bases</code>
</li>
<li>
<b>Field added. </b>
<code>int num_config_regs</code>
</li>
<li>
<b>Field added. </b>
<code>int (*handle_mask_sync)(struct regmap *, int, unsigned int, unsigned int, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_type_config)(unsigned int **, unsigned int, const struct regmap_irq *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*get_irq_reg)(struct regmap_irq_chip_data *, unsigned int, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool mask_writeonly</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int type_reg_stride</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool init_ack_masked</code> ➡️ <code>unsigned int init_ack_masked</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool mask_invert</code> ➡️ <code>unsigned int mask_invert</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool use_ack</code> ➡️ <code>unsigned int use_ack</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool ack_invert</code> ➡️ <code>unsigned int ack_invert</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool clear_ack</code> ➡️ <code>unsigned int clear_ack</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool wake_invert</code> ➡️ <code>unsigned int wake_invert</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool runtime_pm</code> ➡️ <code>unsigned int runtime_pm</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool type_invert</code> ➡️ <code>unsigned int type_invert</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool type_in_mask</code> ➡️ <code>unsigned int type_in_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool clear_on_unmask</code> ➡️ <code>unsigned int clear_on_unmask</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool not_fixed_stride</code> ➡️ <code>unsigned int not_fixed_stride</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool status_invert</code> ➡️ <code>unsigned int status_invert</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int no_status</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int type_base</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int *virt_reg_base</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int mask_invert</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int type_invert</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int not_fixed_stride</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_type_reg</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_virt_regs</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_type_virt)(unsigned int **, unsigned int, long unsigned int, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*handle_mask_sync)(struct regmap *, int, unsigned int, unsigned int, void *)</code> ➡️ <code>int (*handle_mask_sync)(int, unsigned int, unsigned int, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_type_config)(unsigned int **, unsigned int, const struct regmap_irq *, int)</code> ➡️ <code>int (*set_type_config)(unsigned int **, unsigned int, const struct regmap_irq *, int, void *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
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
