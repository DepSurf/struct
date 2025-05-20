# Struct: <code>pwm_chip</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    struct list_head list;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device *pwms;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    bool can_sleep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    struct list_head list;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device *pwms;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    bool can_sleep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    struct list_head list;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device *pwms;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    bool can_sleep;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    struct list_head list;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device *pwms;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    struct list_head list;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device *pwms;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    struct list_head list;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device *pwms;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    struct list_head list;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device *pwms;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    struct module *owner;
    unsigned int id;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    bool atomic;
    struct pwm_device *pwms;
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
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
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
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pwm_chip {
    struct device *dev;
    const struct pwm_ops *ops;
    int base;
    unsigned int npwm;
    struct pwm_device * (*of_xlate)(struct pwm_chip *, const struct of_phandle_args *);
    unsigned int of_pwm_n_cells;
    struct list_head list;
    struct pwm_device *pwms;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool can_sleep</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int id</code>
</li>
<li>
<b>Field added. </b>
<code>bool atomic</code>
</li>
<li>
<b>Field removed. </b>
<code>int base</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head list</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
