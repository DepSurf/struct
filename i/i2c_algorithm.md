# Struct: <code>i2c_algorithm</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
    int (*reg_slave)(struct i2c_client *);
    int (*unreg_slave)(struct i2c_client *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
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
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
    int (*reg_slave)(struct i2c_client *);
    int (*unreg_slave)(struct i2c_client *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
    int (*reg_slave)(struct i2c_client *);
    int (*unreg_slave)(struct i2c_client *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
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
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct i2c_algorithm {
    int (*master_xfer)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int);
    int (*smbus_xfer)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *);
    u32 (*functionality)(struct i2c_adapter *);
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
<code>int (*reg_slave)(struct i2c_client *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*unreg_slave)(struct i2c_client *)</code>
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
<code>int (*reg_slave)(struct i2c_client *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*unreg_slave)(struct i2c_client *)</code>
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
<code>int (*master_xfer_atomic)(struct i2c_adapter *, struct i2c_msg *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*smbus_xfer_atomic)(struct i2c_adapter *, u16, short unsigned int, char, u8, int, union i2c_smbus_data *)</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*reg_slave)(struct i2c_client *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*unreg_slave)(struct i2c_client *)</code>
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
<code>int (*reg_slave)(struct i2c_client *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*unreg_slave)(struct i2c_client *)</code>
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
