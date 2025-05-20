# Struct: <code>ec_params_motion_sense</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ec_params_motion_sense {
    uint8_t cmd;
    struct (anon) dump;
    struct (anon) kb_wake_angle;
    struct (anon) info;
    struct (anon) info_3;
    struct (anon) data;
    struct (anon) fifo_flush;
    struct (anon) perform_calib;
    struct (anon) list_activities;
    struct (anon) ec_rate;
    struct (anon) sensor_odr;
    struct (anon) sensor_range;
    struct (anon) sensor_offset;
    struct (anon) sensor_scale;
    struct (anon) fifo_read;
    struct ec_motion_sense_activity set_activity;
    struct (anon) fifo_int_enable;
    struct (anon) spoof;
    struct (anon) tablet_mode_threshold;
};
```
</details>
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
<b>Regular</b>
<ul>
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
