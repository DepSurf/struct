# Struct: <code>irq_domain_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    void (*activate)(struct irq_domain *, struct irq_data *);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    void (*activate)(struct irq_domain *, struct irq_data *);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    void (*activate)(struct irq_domain *, struct irq_data *);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    void (*activate)(struct irq_domain *, struct irq_data *);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
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
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
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
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct irq_domain_ops {
    int (*match)(struct irq_domain *, struct device_node *, enum irq_domain_bus_token);
    int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token);
    int (*map)(struct irq_domain *, unsigned int, irq_hw_number_t);
    void (*unmap)(struct irq_domain *, unsigned int);
    int (*xlate)(struct irq_domain *, struct device_node *, const u32 *, unsigned int, long unsigned int *, unsigned int *);
    int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *);
    void (*free)(struct irq_domain *, unsigned int, unsigned int);
    int (*activate)(struct irq_domain *, struct irq_data *, bool);
    void (*deactivate)(struct irq_domain *, struct irq_data *);
    int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *);
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
<code>int (*select)(struct irq_domain *, struct irq_fwspec *, enum irq_domain_bus_token)</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>void (*activate)(struct irq_domain *, struct irq_data *)</code> ➡️ <code>int (*activate)(struct irq_domain *, struct irq_data *, bool)</code>
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
<code>int (*alloc)(struct irq_domain *, unsigned int, unsigned int, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*free)(struct irq_domain *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*activate)(struct irq_domain *, struct irq_data *, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*deactivate)(struct irq_domain *, struct irq_data *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*translate)(struct irq_domain *, struct irq_fwspec *, long unsigned int *, unsigned int *)</code>
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
