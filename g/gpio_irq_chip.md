# Struct: <code>gpio_irq_chip</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool need_valid_mask;
    long unsigned int *valid_mask;
    unsigned int first;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool need_valid_mask;
    long unsigned int *valid_mask;
    unsigned int first;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int parent_irq;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool need_valid_mask;
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool need_valid_mask;
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void * (*populate_parent_alloc_arg)(struct gpio_chip *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void * (*populate_parent_alloc_arg)(struct gpio_chip *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void * (*populate_parent_alloc_arg)(struct gpio_chip *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void * (*populate_parent_alloc_arg)(struct gpio_chip *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void * (*populate_parent_alloc_arg)(struct gpio_chip *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    void **parent_handler_data_array;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool per_parent_data;
    bool initialized;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    int (*populate_parent_alloc_arg)(struct gpio_chip *, union gpio_irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    void **parent_handler_data_array;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool per_parent_data;
    bool initialized;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    int (*populate_parent_alloc_arg)(struct gpio_chip *, union gpio_irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    void **parent_handler_data_array;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool per_parent_data;
    bool initialized;
    bool domain_is_allocated_externally;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    int (*populate_parent_alloc_arg)(struct gpio_chip *, union gpio_irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    void **parent_handler_data_array;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    bool per_parent_data;
    bool initialized;
    bool domain_is_allocated_externally;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
    void (*irq_unmask)(struct irq_data *);
    void (*irq_mask)(struct irq_data *);
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
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
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
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct gpio_irq_chip {
    struct irq_chip *chip;
    struct irq_domain *domain;
    const struct irq_domain_ops *domain_ops;
    struct fwnode_handle *fwnode;
    struct irq_domain *parent_domain;
    int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *);
    void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int);
    unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int);
    struct irq_domain_ops child_irq_domain_ops;
    irq_flow_handler_t handler;
    unsigned int default_type;
    struct lock_class_key *lock_key;
    struct lock_class_key *request_key;
    irq_flow_handler_t parent_handler;
    void *parent_handler_data;
    unsigned int num_parents;
    unsigned int *parents;
    unsigned int *map;
    bool threaded;
    int (*init_hw)(struct gpio_chip *);
    void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int);
    long unsigned int *valid_mask;
    unsigned int first;
    void (*irq_enable)(struct irq_data *);
    void (*irq_disable)(struct irq_data *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int parent_irq</code>
</li>
<li>
<b>Field added. </b>
<code>void (*irq_enable)(struct irq_data *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*irq_disable)(struct irq_data *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int parent_irq</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fwnode_handle *fwnode</code>
</li>
<li>
<b>Field added. </b>
<code>struct irq_domain *parent_domain</code>
</li>
<li>
<b>Field added. </b>
<code>int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>struct irq_domain_ops child_irq_domain_ops</code>
</li>
<li>
<b>Field added. </b>
<code>int (*init_hw)(struct gpio_chip *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*init_valid_mask)(struct gpio_chip *, long unsigned int *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool need_valid_mask</code>
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
<code>void * (*populate_parent_alloc_arg)(struct gpio_chip *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*irq_unmask)(struct irq_data *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*irq_mask)(struct irq_data *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int)</code>
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
<code>void **parent_handler_data_array</code>
</li>
<li>
<b>Field added. </b>
<code>bool per_parent_data</code>
</li>
<li>
<b>Field added. </b>
<code>bool initialized</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void * (*populate_parent_alloc_arg)(struct gpio_chip *, unsigned int, unsigned int)</code> ➡️ <code>int (*populate_parent_alloc_arg)(struct gpio_chip *, union gpio_irq_fwspec *, unsigned int, unsigned int)</code>
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
<code>bool domain_is_allocated_externally</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct irq_domain_ops *domain_ops</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct fwnode_handle *fwnode</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_domain *parent_domain</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*child_to_parent_hwirq)(struct gpio_chip *, unsigned int, unsigned int, unsigned int *, unsigned int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*populate_parent_fwspec)(struct gpio_chip *, struct irq_fwspec *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int (*child_offset_to_irq)(struct gpio_chip *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_domain_ops child_irq_domain_ops</code>
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
