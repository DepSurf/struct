# Struct: <code>powercap_zone_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
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
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
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
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct powercap_zone_ops {
    int (*get_max_energy_range_uj)(struct powercap_zone *, u64 *);
    int (*get_energy_uj)(struct powercap_zone *, u64 *);
    int (*reset_energy_uj)(struct powercap_zone *);
    int (*get_max_power_range_uw)(struct powercap_zone *, u64 *);
    int (*get_power_uw)(struct powercap_zone *, u64 *);
    int (*set_enable)(struct powercap_zone *, bool);
    int (*get_enable)(struct powercap_zone *, bool *);
    int (*release)(struct powercap_zone *);
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
