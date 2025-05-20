# Struct: <code>power_supply_desc</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    const enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    const enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
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
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
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
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct power_supply_desc {
    const char *name;
    enum power_supply_type type;
    enum power_supply_usb_type *usb_types;
    size_t num_usb_types;
    enum power_supply_property *properties;
    size_t num_properties;
    int (*get_property)(struct power_supply *, enum power_supply_property, union power_supply_propval *);
    int (*set_property)(struct power_supply *, enum power_supply_property, const union power_supply_propval *);
    int (*property_is_writeable)(struct power_supply *, enum power_supply_property);
    void (*external_power_changed)(struct power_supply *);
    void (*set_charged)(struct power_supply *);
    bool no_thermal;
    int use_for_apm;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum power_supply_usb_type *usb_types</code>
</li>
<li>
<b>Field added. </b>
<code>size_t num_usb_types</code>
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
<b>Field type changed. </b>
<code>enum power_supply_usb_type *usb_types</code> ➡️ <code>const enum power_supply_usb_type *usb_types</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum power_supply_property *properties</code> ➡️ <code>const enum power_supply_property *properties</code>
</li>
</ul>
</details>
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
