# Struct: <code>rio_switch_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
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
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
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
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rio_switch_ops {
    struct module *owner;
    int (*add_entry)(struct rio_mport *, u16, u8, u16, u16, u8);
    int (*get_entry)(struct rio_mport *, u16, u8, u16, u16, u8 *);
    int (*clr_table)(struct rio_mport *, u16, u8, u16);
    int (*set_domain)(struct rio_mport *, u16, u8, u8);
    int (*get_domain)(struct rio_mport *, u16, u8, u8 *);
    int (*em_init)(struct rio_dev *);
    int (*em_handle)(struct rio_dev *, u8);
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
