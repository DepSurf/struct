# Struct: <code>apic_chip_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg cfg;
    cpumask_var_t domain;
    cpumask_var_t old_domain;
    u8 move_in_progress;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg cfg;
    cpumask_var_t domain;
    cpumask_var_t old_domain;
    u8 move_in_progress;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg cfg;
    cpumask_var_t domain;
    cpumask_var_t old_domain;
    u8 move_in_progress;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg cfg;
    cpumask_var_t domain;
    cpumask_var_t old_domain;
    u8 move_in_progress;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct apic_chip_data {
    struct irq_cfg hw_irq_cfg;
    unsigned int vector;
    unsigned int prev_vector;
    unsigned int cpu;
    unsigned int prev_cpu;
    unsigned int irq;
    struct hlist_node clist;
    unsigned int move_in_progress;
    unsigned int is_managed;
    unsigned int can_reserve;
    unsigned int has_reserved;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct irq_cfg hw_irq_cfg</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int vector</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int prev_vector</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cpu</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int prev_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int irq</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node clist</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int is_managed</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int can_reserve</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int has_reserved</code>
</li>
<li>
<b>Field removed. </b>
<code>struct irq_cfg cfg</code>
</li>
<li>
<b>Field removed. </b>
<code>cpumask_var_t domain</code>
</li>
<li>
<b>Field removed. </b>
<code>cpumask_var_t old_domain</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 move_in_progress</code> ➡️ <code>unsigned int move_in_progress</code>
</li>
</ul>
</details>
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
<b>Arch</b>
<ul>
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
