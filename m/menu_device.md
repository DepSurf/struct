# Struct: <code>menu_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    unsigned int next_timer_us;
    unsigned int predicted_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    unsigned int next_timer_us;
    unsigned int predicted_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    unsigned int next_timer_us;
    unsigned int predicted_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    unsigned int next_timer_us;
    unsigned int predicted_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    unsigned int next_timer_us;
    unsigned int predicted_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int predicted_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct menu_device {
    int last_state_idx;
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    u64 next_timer_ns;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
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
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct menu_device {
    int needs_update;
    int tick_wakeup;
    unsigned int next_timer_us;
    unsigned int bucket;
    unsigned int correction_factor[12];
    unsigned int intervals[8];
    int interval_ptr;
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
<code>int tick_wakeup</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int predicted_us</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int last_state_idx</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 next_timer_ns</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int next_timer_us</code>
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
