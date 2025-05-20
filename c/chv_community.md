# Struct: <code>chv_community</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct chv_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t ngpios;
    size_t nirqs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct chv_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t ngpios;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct chv_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct chv_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct intel_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct intel_padgroup *gpps;
    size_t ngpps;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct chv_community {
    const char *uid;
    const struct pinctrl_pin_desc *pins;
    size_t npins;
    const struct chv_pingroup *groups;
    size_t ngroups;
    const struct intel_function *functions;
    size_t nfunctions;
    const struct chv_gpio_pinrange *gpio_ranges;
    size_t ngpio_ranges;
    size_t nirqs;
    acpi_adr_space_type acpi_space_id;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>acpi_adr_space_type acpi_space_id</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>size_t ngpios</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>const struct chv_function *functions</code> ➡️ <code>const struct intel_function *functions</code>
</li>
</ul>
</details>
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
<code>const struct intel_padgroup *gpps</code>
</li>
<li>
<b>Field added. </b>
<code>size_t ngpps</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct chv_gpio_pinrange *gpio_ranges</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t ngpio_ranges</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct chv_pingroup *groups</code> ➡️ <code>const struct intel_pingroup *groups</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
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
