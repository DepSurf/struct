# Struct: <code>thermal_zone_device_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    void (*hot)(struct thermal_zone_device *);
    void (*critical)(struct thermal_zone_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    void (*hot)(struct thermal_zone_device *);
    void (*critical)(struct thermal_zone_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    void (*hot)(struct thermal_zone_device *);
    void (*critical)(struct thermal_zone_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    void (*hot)(struct thermal_zone_device *);
    void (*critical)(struct thermal_zone_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    void (*hot)(struct thermal_zone_device *);
    void (*critical)(struct thermal_zone_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    void (*hot)(struct thermal_zone_device *);
    void (*critical)(struct thermal_zone_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, const struct thermal_trip *, enum thermal_trend *);
    void (*hot)(struct thermal_zone_device *);
    void (*critical)(struct thermal_zone_device *);
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
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
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
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct thermal_zone_device_ops {
    int (*bind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*unbind)(struct thermal_zone_device *, struct thermal_cooling_device *);
    int (*get_temp)(struct thermal_zone_device *, int *);
    int (*set_trips)(struct thermal_zone_device *, int, int);
    int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *);
    int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode);
    int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *);
    int (*get_trip_temp)(struct thermal_zone_device *, int, int *);
    int (*set_trip_temp)(struct thermal_zone_device *, int, int);
    int (*get_trip_hyst)(struct thermal_zone_device *, int, int *);
    int (*set_trip_hyst)(struct thermal_zone_device *, int, int);
    int (*get_crit_temp)(struct thermal_zone_device *, int *);
    int (*set_emul_temp)(struct thermal_zone_device *, int);
    int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *);
    int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type);
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*set_trips)(struct thermal_zone_device *, int, int)</code>
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
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*change_mode)(struct thermal_zone_device *, enum thermal_device_mode)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*hot)(struct thermal_zone_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*critical)(struct thermal_zone_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_mode)(struct thermal_zone_device *, enum thermal_device_mode *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_mode)(struct thermal_zone_device *, enum thermal_device_mode)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*notify)(struct thermal_zone_device *, int, enum thermal_trip_type)</code>
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
<b>Field removed. </b>
<code>int (*get_trip_type)(struct thermal_zone_device *, int, enum thermal_trip_type *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_trip_temp)(struct thermal_zone_device *, int, int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_trip_hyst)(struct thermal_zone_device *, int, int *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_trend)(struct thermal_zone_device *, int, enum thermal_trend *)</code> ➡️ <code>int (*get_trend)(struct thermal_zone_device *, const struct thermal_trip *, enum thermal_trend *)</code>
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
