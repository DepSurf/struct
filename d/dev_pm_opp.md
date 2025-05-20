# Struct: <code>dev_pm_opp</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    bool removed;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    bool removed;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    bool removed;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    bool removed;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
    const char *of_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    bool removed;
    unsigned int pstate;
    long unsigned int *rates;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
    const char *of_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    bool removed;
    long unsigned int *rates;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
    const char *of_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    bool removed;
    long unsigned int *rates;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    struct dev_pm_opp_icc_bw *bandwidth;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
    const char *of_name;
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
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
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
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dev_pm_opp {
    struct list_head node;
    struct kref kref;
    bool available;
    bool dynamic;
    bool turbo;
    bool suspend;
    unsigned int pstate;
    long unsigned int rate;
    unsigned int level;
    struct dev_pm_opp_supply *supplies;
    long unsigned int clock_latency_ns;
    struct dev_pm_opp **required_opps;
    struct opp_table *opp_table;
    struct device_node *np;
    struct dentry *dentry;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct dev_pm_opp **required_opps</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int level</code>
</li>
</ul>
</details>
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
<code>struct dev_pm_opp_icc_bw *bandwidth</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool removed</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const char *of_name</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int *rates</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int rate</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int pstate</code>
</li>
</ul>
</details>
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
