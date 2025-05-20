# Struct: <code>rdt_domain</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    u32 *cbm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 new_ctrl;
    bool have_new_ctrl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 new_ctrl;
    bool have_new_ctrl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    struct pseudo_lock_region *plr;
    struct resctrl_staged_config staged_config[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    struct pseudo_lock_region *plr;
    struct resctrl_staged_config staged_config[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    struct pseudo_lock_region *plr;
    struct resctrl_staged_config staged_config[3];
    u32 *mbps_val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    struct pseudo_lock_region *plr;
    struct resctrl_staged_config staged_config[3];
    u32 *mbps_val;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    struct pseudo_lock_region *plr;
    struct resctrl_staged_config staged_config[3];
    u32 *mbps_val;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rdt_domain {
    struct list_head list;
    int id;
    struct cpumask cpu_mask;
    long unsigned int *rmid_busy_llc;
    struct mbm_state *mbm_total;
    struct mbm_state *mbm_local;
    struct delayed_work mbm_over;
    struct delayed_work cqm_limbo;
    int mbm_work_cpu;
    int cqm_work_cpu;
    u32 *ctrl_val;
    u32 *mbps_val;
    u32 new_ctrl;
    bool have_new_ctrl;
    struct pseudo_lock_region *plr;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int *rmid_busy_llc</code>
</li>
<li>
<b>Field added. </b>
<code>struct mbm_state *mbm_total</code>
</li>
<li>
<b>Field added. </b>
<code>struct mbm_state *mbm_local</code>
</li>
<li>
<b>Field added. </b>
<code>struct delayed_work mbm_over</code>
</li>
<li>
<b>Field added. </b>
<code>struct delayed_work cqm_limbo</code>
</li>
<li>
<b>Field added. </b>
<code>int mbm_work_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>int cqm_work_cpu</code>
</li>
<li>
<b>Field added. </b>
<code>u32 *ctrl_val</code>
</li>
<li>
<b>Field added. </b>
<code>u32 new_ctrl</code>
</li>
<li>
<b>Field added. </b>
<code>bool have_new_ctrl</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 *cbm</code>
</li>
</ul>
</details>
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
<code>u32 *mbps_val</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct pseudo_lock_region *plr</code>
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct resctrl_staged_config staged_config[3]</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 *ctrl_val</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 *mbps_val</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 new_ctrl</code>
</li>
<li>
<b>Field removed. </b>
<code>bool have_new_ctrl</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 *mbps_val</code>
</li>
</ul>
</details>
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
