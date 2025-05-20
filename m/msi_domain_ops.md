# Struct: <code>msi_domain_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
    int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int);
    void (*domain_free_irqs)(struct irq_domain *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
    int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int);
    void (*domain_free_irqs)(struct irq_domain *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
    int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int);
    void (*domain_free_irqs)(struct irq_domain *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int);
    void (*domain_free_irqs)(struct irq_domain *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*prepare_desc)(struct irq_domain *, msi_alloc_info_t *, struct msi_desc *);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int);
    void (*domain_free_irqs)(struct irq_domain *, struct device *);
    void (*msi_post_free)(struct irq_domain *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*prepare_desc)(struct irq_domain *, msi_alloc_info_t *, struct msi_desc *);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int);
    void (*domain_free_irqs)(struct irq_domain *, struct device *);
    void (*msi_post_free)(struct irq_domain *, struct device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*prepare_desc)(struct irq_domain *, msi_alloc_info_t *, struct msi_desc *);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int);
    void (*domain_free_irqs)(struct irq_domain *, struct device *);
    void (*msi_post_free)(struct irq_domain *, struct device *);
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
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
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
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct msi_domain_ops {
    irq_hw_number_t (*get_hwirq)(struct msi_domain_info *, msi_alloc_info_t *);
    int (*msi_init)(struct irq_domain *, struct msi_domain_info *, unsigned int, irq_hw_number_t, msi_alloc_info_t *);
    void (*msi_free)(struct irq_domain *, struct msi_domain_info *, unsigned int);
    int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *);
    int (*msi_prepare)(struct irq_domain *, struct device *, int, msi_alloc_info_t *);
    void (*msi_finish)(msi_alloc_info_t *, int);
    void (*set_desc)(msi_alloc_info_t *, struct msi_desc *);
    int (*handle_error)(struct irq_domain *, struct msi_desc *, int);
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*domain_alloc_irqs)(struct irq_domain *, struct device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*domain_free_irqs)(struct irq_domain *, struct device *)</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>void (*msi_finish)(msi_alloc_info_t *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*handle_error)(struct irq_domain *, struct msi_desc *, int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*prepare_desc)(struct irq_domain *, msi_alloc_info_t *, struct msi_desc *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*msi_post_free)(struct irq_domain *, struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*msi_check)(struct irq_domain *, struct msi_domain_info *, struct device *)</code>
</li>
</ul>
</details>
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
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
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
