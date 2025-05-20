# Struct: <code>i2c_client</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int irq;
    struct list_head detected;
    i2c_slave_cb_t slave_cb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    void *devres_group_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    void *devres_group_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    void *devres_group_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    void *devres_group_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    void *devres_group_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    void *devres_group_id;
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
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    i2c_slave_cb_t slave_cb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
    i2c_slave_cb_t slave_cb;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
};
```
</details>
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
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct i2c_client {
    short unsigned int flags;
    short unsigned int addr;
    char name[20];
    struct i2c_adapter *adapter;
    struct device dev;
    int init_irq;
    int irq;
    struct list_head detected;
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
<code>i2c_slave_cb_t slave_cb</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>i2c_slave_cb_t slave_cb</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int init_irq</code>
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *devres_group_id</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>i2c_slave_cb_t slave_cb</code>
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
<code>i2c_slave_cb_t slave_cb</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
