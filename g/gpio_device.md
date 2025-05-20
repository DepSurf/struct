# Struct: <code>gpio_device</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct atomic_notifier_head notifier;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct blocking_notifier_head notifier;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct blocking_notifier_head notifier;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct blocking_notifier_head notifier;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct blocking_notifier_head notifier;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct gpio_device {
    struct device dev;
    struct cdev chrdev;
    int id;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct blocking_notifier_head notifier;
    struct rw_semaphore sem;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct gpio_device {
    struct device dev;
    struct cdev chrdev;
    int id;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct blocking_notifier_head notifier;
    struct rw_semaphore sem;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct gpio_device {
    struct device dev;
    struct cdev chrdev;
    int id;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct blocking_notifier_head line_state_notifier;
    struct blocking_notifier_head device_notifier;
    struct rw_semaphore sem;
    struct list_head pin_ranges;
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
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
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
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct gpio_device {
    int id;
    struct device dev;
    struct cdev chrdev;
    struct device *mockdev;
    struct module *owner;
    struct gpio_chip *chip;
    struct gpio_desc *descs;
    int base;
    u16 ngpio;
    const char *label;
    void *data;
    struct list_head list;
    struct list_head pin_ranges;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char *label</code> ➡️ <code>const char *label</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct atomic_notifier_head notifier</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct atomic_notifier_head notifier</code> ➡️ <code>struct blocking_notifier_head notifier</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rw_semaphore sem</code>
</li>
</ul>
</details>
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
<code>struct blocking_notifier_head line_state_notifier</code>
</li>
<li>
<b>Field added. </b>
<code>struct blocking_notifier_head device_notifier</code>
</li>
<li>
<b>Field removed. </b>
<code>struct blocking_notifier_head notifier</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
