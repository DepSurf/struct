# Struct: <code>thermal_zone_of_device_ops</code>

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
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
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
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct thermal_zone_of_device_ops {
    int (*get_temp)(void *, int *);
    int (*get_trend)(void *, int, enum thermal_trend *);
    int (*set_trips)(void *, int, int);
    int (*set_emul_temp)(void *, int);
    int (*set_trip_temp)(void *, int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct thermal_zone_of_device_ops {
    int (*get_temp)(void *, int *);
    int (*get_trend)(void *, int, enum thermal_trend *);
    int (*set_trips)(void *, int, int);
    int (*set_emul_temp)(void *, int);
    int (*set_trip_temp)(void *, int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct thermal_zone_of_device_ops {
    int (*get_temp)(void *, int *);
    int (*get_trend)(void *, int, enum thermal_trend *);
    int (*set_trips)(void *, int, int);
    int (*set_emul_temp)(void *, int);
    int (*set_trip_temp)(void *, int, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct thermal_zone_of_device_ops {
    int (*get_temp)(void *, int *);
    int (*get_trend)(void *, int, enum thermal_trend *);
    int (*set_trips)(void *, int, int);
    int (*set_emul_temp)(void *, int);
    int (*set_trip_temp)(void *, int, int);
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
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Arch</b>
<ul>
</ul>
