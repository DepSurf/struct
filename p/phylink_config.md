# Struct: <code>phylink_config</code>

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
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool pcs_poll;
    bool poll_fixed_state;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool pcs_poll;
    bool poll_fixed_state;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool pcs_poll;
    bool poll_fixed_state;
    bool ovr_an_inband;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool pcs_poll;
    bool poll_fixed_state;
    bool ovr_an_inband;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool legacy_pre_march2020;
    bool poll_fixed_state;
    bool ovr_an_inband;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
    long unsigned int supported_interfaces[1];
    long unsigned int mac_capabilities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool legacy_pre_march2020;
    bool poll_fixed_state;
    bool mac_managed_pm;
    bool ovr_an_inband;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
    long unsigned int supported_interfaces[1];
    long unsigned int mac_capabilities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool legacy_pre_march2020;
    bool poll_fixed_state;
    bool mac_managed_pm;
    bool ovr_an_inband;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
    long unsigned int supported_interfaces[1];
    long unsigned int mac_capabilities;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
    bool poll_fixed_state;
    bool mac_managed_pm;
    bool ovr_an_inband;
    void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *);
    long unsigned int supported_interfaces[1];
    long unsigned int mac_capabilities;
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
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
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
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct phylink_config {
    struct device *dev;
    enum phylink_op_type type;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool pcs_poll</code>
</li>
<li>
<b>Field added. </b>
<code>bool poll_fixed_state</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_fixed_state)(struct phylink_config *, struct phylink_link_state *)</code>
</li>
</ul>
</details>
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
<code>bool ovr_an_inband</code>
</li>
</ul>
</details>
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
<code>bool legacy_pre_march2020</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int supported_interfaces[1]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int mac_capabilities</code>
</li>
<li>
<b>Field removed. </b>
<code>bool pcs_poll</code>
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
<code>bool mac_managed_pm</code>
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
<b>Field removed. </b>
<code>bool legacy_pre_march2020</code>
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
