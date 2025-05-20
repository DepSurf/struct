# Struct: <code>gpio_chip</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct device *dev;
    struct device *cdev;
    struct module *owner;
    struct list_head list;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_debounce)(struct gpio_chip *, unsigned int, unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int base;
    u16 ngpio;
    struct gpio_desc *desc;
    const const char * *names;
    bool can_sleep;
    bool irq_not_threaded;
    struct irq_chip *irqchip;
    struct irq_domain *irqdomain;
    unsigned int irq_base;
    irq_flow_handler_t irq_handler;
    unsigned int irq_default_type;
    int irq_parent;
    struct lock_class_key *lock_key;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_debounce)(struct gpio_chip *, unsigned int, unsigned int);
    int (*set_single_ended)(struct gpio_chip *, unsigned int, enum single_ended_mode);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    bool irq_not_threaded;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    long unsigned int (*pin2mask)(struct gpio_chip *, unsigned int);
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct irq_chip *irqchip;
    struct irq_domain *irqdomain;
    unsigned int irq_base;
    irq_flow_handler_t irq_handler;
    unsigned int irq_default_type;
    int irq_parent;
    struct lock_class_key *lock_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_debounce)(struct gpio_chip *, unsigned int, unsigned int);
    int (*set_single_ended)(struct gpio_chip *, unsigned int, enum single_ended_mode);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    long unsigned int (*pin2mask)(struct gpio_chip *, unsigned int);
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct irq_chip *irqchip;
    struct irq_domain *irqdomain;
    unsigned int irq_base;
    irq_flow_handler_t irq_handler;
    unsigned int irq_default_type;
    int irq_chained_parent;
    bool irq_nested;
    bool irq_need_valid_mask;
    long unsigned int *irq_valid_mask;
    struct lock_class_key *lock_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    long unsigned int (*pin2mask)(struct gpio_chip *, unsigned int);
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct irq_chip *irqchip;
    struct irq_domain *irqdomain;
    unsigned int irq_base;
    irq_flow_handler_t irq_handler;
    unsigned int irq_default_type;
    unsigned int irq_chained_parent;
    bool irq_nested;
    bool irq_need_valid_mask;
    long unsigned int *irq_valid_mask;
    struct lock_class_key *lock_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    bool need_valid_mask;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir;
    bool bgpio_dir_inverted;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    bool need_valid_mask;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    bool need_valid_mask;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int base;
    u16 ngpio;
    u16 offset;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct fwnode_handle *fwnode;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int (*en_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int (*dis_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int base;
    u16 ngpio;
    u16 offset;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    raw_spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct fwnode_handle *fwnode;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int (*en_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int (*dis_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int base;
    u16 ngpio;
    u16 offset;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    raw_spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct fwnode_handle *fwnode;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int (*en_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int (*dis_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int base;
    u16 ngpio;
    u16 offset;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    raw_spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct fwnode_handle *fwnode;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int (*add_pin_ranges)(struct gpio_chip *);
    int (*en_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int (*dis_hw_timestamp)(struct gpio_chip *, u32, long unsigned int);
    int base;
    u16 ngpio;
    u16 offset;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    raw_spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
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
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
    struct device_node *of_node;
    unsigned int of_gpio_n_cells;
    int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
    struct device_node *of_node;
    unsigned int of_gpio_n_cells;
    int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
    struct device_node *of_node;
    unsigned int of_gpio_n_cells;
    int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
    struct device_node *of_node;
    unsigned int of_gpio_n_cells;
    int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *);
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
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct gpio_chip {
    const char *label;
    struct gpio_device *gpiodev;
    struct device *parent;
    struct module *owner;
    int (*request)(struct gpio_chip *, unsigned int);
    void (*free)(struct gpio_chip *, unsigned int);
    int (*get_direction)(struct gpio_chip *, unsigned int);
    int (*direction_input)(struct gpio_chip *, unsigned int);
    int (*direction_output)(struct gpio_chip *, unsigned int, int);
    int (*get)(struct gpio_chip *, unsigned int);
    int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    void (*set)(struct gpio_chip *, unsigned int, int);
    void (*set_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *);
    int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int);
    int (*to_irq)(struct gpio_chip *, unsigned int);
    void (*dbg_show)(struct seq_file *, struct gpio_chip *);
    int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    int base;
    u16 ngpio;
    const const char * *names;
    bool can_sleep;
    long unsigned int (*read_reg)(void *);
    void (*write_reg)(void *, long unsigned int);
    bool be_bits;
    void *reg_dat;
    void *reg_set;
    void *reg_clr;
    void *reg_dir_out;
    void *reg_dir_in;
    bool bgpio_dir_unreadable;
    int bgpio_bits;
    spinlock_t bgpio_lock;
    long unsigned int bgpio_data;
    long unsigned int bgpio_dir;
    struct gpio_irq_chip irq;
    long unsigned int *valid_mask;
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
<code>struct gpio_device *gpiodev</code>
</li>
<li>
<b>Field added. </b>
<code>struct device *parent</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_single_ended)(struct gpio_chip *, unsigned int, enum single_ended_mode)</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int (*read_reg)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*write_reg)(void *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int (*pin2mask)(struct gpio_chip *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void *reg_dat</code>
</li>
<li>
<b>Field added. </b>
<code>void *reg_set</code>
</li>
<li>
<b>Field added. </b>
<code>void *reg_clr</code>
</li>
<li>
<b>Field added. </b>
<code>void *reg_dir</code>
</li>
<li>
<b>Field added. </b>
<code>int bgpio_bits</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t bgpio_lock</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int bgpio_data</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int bgpio_dir</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *dev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct device *cdev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct gpio_desc *desc</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head pin_ranges</code>
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
<code>int irq_chained_parent</code>
</li>
<li>
<b>Field added. </b>
<code>bool irq_nested</code>
</li>
<li>
<b>Field added. </b>
<code>bool irq_need_valid_mask</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int *irq_valid_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>bool irq_not_threaded</code>
</li>
<li>
<b>Field removed. </b>
<code>int irq_parent</code>
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
<code>int (*set_config)(struct gpio_chip *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_debounce)(struct gpio_chip *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_single_ended)(struct gpio_chip *, unsigned int, enum single_ended_mode)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int irq_chained_parent</code> ➡️ <code>unsigned int irq_chained_parent</code>
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
<code>int (*get_multiple)(struct gpio_chip *, long unsigned int *, long unsigned int *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool be_bits</code>
</li>
<li>
<b>Field added. </b>
<code>struct gpio_irq_chip irq</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int (*pin2mask)(struct gpio_chip *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_chip *irqchip</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_domain *irqdomain</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int irq_base</code>
</li>
<li>
<b>Field removed. </b>
<code>irq_flow_handler_t irq_handler</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int irq_default_type</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int irq_chained_parent</code>
</li>
<li>
<b>Field removed. </b>
<code>bool irq_nested</code>
</li>
<li>
<b>Field removed. </b>
<code>bool irq_need_valid_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int *irq_valid_mask</code>
</li>
<li>
<b>Field removed. </b>
<code>struct lock_class_key *lock_key</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool need_valid_mask</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int *valid_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*init_valid_mask)(struct gpio_chip *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool bgpio_dir_inverted</code>
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
<code>void *reg_dir_out</code>
</li>
<li>
<b>Field added. </b>
<code>void *reg_dir_in</code>
</li>
<li>
<b>Field added. </b>
<code>bool bgpio_dir_unreadable</code>
</li>
<li>
<b>Field removed. </b>
<code>void *reg_dir</code>
</li>
<li>
<b>Field removed. </b>
<code>bool bgpio_dir_inverted</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool need_valid_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*init_valid_mask)(struct gpio_chip *)</code> ➡️ <code>int (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*add_pin_ranges)(struct gpio_chip *)</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 offset</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fwnode_handle *fwnode</code>
</li>
<li>
<b>Field added. </b>
<code>int (*en_hw_timestamp)(struct gpio_chip *, u32, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dis_hw_timestamp)(struct gpio_chip *, u32, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>spinlock_t bgpio_lock</code> ➡️ <code>raw_spinlock_t bgpio_lock</code>
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
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device_node *of_node</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int of_gpio_n_cells</code>
</li>
<li>
<b>Field added. </b>
<code>int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device_node *of_node</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int of_gpio_n_cells</code>
</li>
<li>
<b>Field added. </b>
<code>int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device_node *of_node</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int of_gpio_n_cells</code>
</li>
<li>
<b>Field added. </b>
<code>int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct device_node *of_node</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int of_gpio_n_cells</code>
</li>
<li>
<b>Field added. </b>
<code>int (*of_xlate)(struct gpio_chip *, const struct of_phandle_args *, u32 *)</code>
</li>
</ul>
</details>
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
