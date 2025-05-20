# Struct: <code>dbs_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dbs_data {
    struct common_dbs_data *cdata;
    unsigned int min_sampling_rate;
    int usage_count;
    void *tuners;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int min_sampling_rate;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int min_sampling_rate;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int min_sampling_rate;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    struct dbs_governor *gov;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    struct dbs_governor *gov;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    struct dbs_governor *gov;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    struct dbs_governor *gov;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
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
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
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
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dbs_data {
    struct gov_attr_set attr_set;
    void *tuners;
    unsigned int ignore_nice_load;
    unsigned int sampling_rate;
    unsigned int sampling_down_factor;
    unsigned int up_threshold;
    unsigned int io_is_busy;
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
<code>struct gov_attr_set attr_set</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int ignore_nice_load</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int sampling_rate</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int sampling_down_factor</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int up_threshold</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int io_is_busy</code>
</li>
<li>
<b>Field removed. </b>
<code>struct common_dbs_data *cdata</code>
</li>
<li>
<b>Field removed. </b>
<code>int usage_count</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int min_sampling_rate</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dbs_governor *gov</code>
</li>
</ul>
</details>
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
