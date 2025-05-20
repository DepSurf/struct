# Struct: <code>mmc_bus_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*power_save)(struct mmc_host *);
    int (*power_restore)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*power_save)(struct mmc_host *);
    int (*power_restore)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*power_save)(struct mmc_host *);
    int (*power_restore)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*power_save)(struct mmc_host *);
    int (*power_restore)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*power_save)(struct mmc_host *);
    int (*power_restore)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*power_save)(struct mmc_host *);
    int (*power_restore)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
    bool (*cache_enabled)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
    bool (*cache_enabled)(struct mmc_host *);
    int (*flush_cache)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
    bool (*cache_enabled)(struct mmc_host *);
    int (*flush_cache)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
    bool (*cache_enabled)(struct mmc_host *);
    int (*flush_cache)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
    bool (*cache_enabled)(struct mmc_host *);
    int (*flush_cache)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
    bool (*cache_enabled)(struct mmc_host *);
    int (*flush_cache)(struct mmc_host *);
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
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
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
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmc_bus_ops {
    void (*remove)(struct mmc_host *);
    void (*detect)(struct mmc_host *);
    int (*pre_suspend)(struct mmc_host *);
    int (*suspend)(struct mmc_host *);
    int (*resume)(struct mmc_host *);
    int (*runtime_suspend)(struct mmc_host *);
    int (*runtime_resume)(struct mmc_host *);
    int (*alive)(struct mmc_host *);
    int (*shutdown)(struct mmc_host *);
    int (*hw_reset)(struct mmc_host *);
    int (*sw_reset)(struct mmc_host *);
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
<code>int (*hw_reset)(struct mmc_host *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*sw_reset)(struct mmc_host *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*reset)(struct mmc_host *)</code>
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
<code>int (*power_save)(struct mmc_host *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*power_restore)(struct mmc_host *)</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
<code>bool (*cache_enabled)(struct mmc_host *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*flush_cache)(struct mmc_host *)</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
