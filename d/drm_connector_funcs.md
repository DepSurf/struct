# Struct: <code>drm_connector_funcs</code>

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
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
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
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
    void (*oob_hotplug_event)(struct drm_connector *, enum drm_connector_status);
    void (*debugfs_init)(struct drm_connector *, struct dentry *);
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
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
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
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct drm_connector_funcs {
    int (*dpms)(struct drm_connector *, int);
    void (*reset)(struct drm_connector *);
    enum drm_connector_status (*detect)(struct drm_connector *, bool);
    void (*force)(struct drm_connector *);
    int (*fill_modes)(struct drm_connector *, uint32_t, uint32_t);
    int (*set_property)(struct drm_connector *, struct drm_property *, uint64_t);
    int (*late_register)(struct drm_connector *);
    void (*early_unregister)(struct drm_connector *);
    void (*destroy)(struct drm_connector *);
    struct drm_connector_state * (*atomic_duplicate_state)(struct drm_connector *);
    void (*atomic_destroy_state)(struct drm_connector *, struct drm_connector_state *);
    int (*atomic_set_property)(struct drm_connector *, struct drm_connector_state *, struct drm_property *, uint64_t);
    int (*atomic_get_property)(struct drm_connector *, const struct drm_connector_state *, struct drm_property *, uint64_t *);
    void (*atomic_print_state)(struct drm_printer *, const struct drm_connector_state *);
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
