# Struct: <code>rdt_resource</code>

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
struct rdt_resource {
    bool enabled;
    bool capable;
    char *name;
    int num_closid;
    int cbm_len;
    int min_cbm_bits;
    u32 max_cbm;
    struct list_head domains;
    int num_domains;
    int msr_base;
    u32 *tmp_cbms;
    int num_tmp_cbms;
    int cache_level;
    int cbm_idx_multi;
    int cbm_idx_offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(char *, struct rdt_resource *, struct rdt_domain *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(char *, struct rdt_resource *, struct rdt_domain *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(char *, struct rdt_resource *, struct rdt_domain *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    unsigned int mbm_width;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    unsigned int mbm_width;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    unsigned int mbm_width;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    int num_rmid;
    int cache_level;
    struct resctrl_cache cache;
    struct resctrl_membw membw;
    struct list_head domains;
    char *name;
    int data_width;
    u32 default_ctrl;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct resctrl_schema *, struct rdt_domain *);
    struct list_head evt_list;
    long unsigned int fflags;
    bool cdp_capable;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    int num_rmid;
    int cache_level;
    struct resctrl_cache cache;
    struct resctrl_membw membw;
    struct list_head domains;
    char *name;
    int data_width;
    u32 default_ctrl;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct resctrl_schema *, struct rdt_domain *);
    struct list_head evt_list;
    long unsigned int fflags;
    bool cdp_capable;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_capable;
    bool mon_capable;
    int num_rmid;
    int cache_level;
    struct resctrl_cache cache;
    struct resctrl_membw membw;
    struct list_head domains;
    char *name;
    int data_width;
    u32 default_ctrl;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct resctrl_schema *, struct rdt_domain *);
    struct list_head evt_list;
    long unsigned int fflags;
    bool cdp_capable;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_capable;
    bool mon_capable;
    int num_rmid;
    int cache_level;
    struct resctrl_cache cache;
    struct resctrl_membw membw;
    struct list_head domains;
    char *name;
    int data_width;
    u32 default_ctrl;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct resctrl_schema *, struct rdt_domain *);
    struct list_head evt_list;
    long unsigned int fflags;
    bool cdp_capable;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_capable;
    bool mon_capable;
    int num_rmid;
    int cache_level;
    struct resctrl_cache cache;
    struct resctrl_membw membw;
    struct list_head domains;
    char *name;
    int data_width;
    u32 default_ctrl;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct resctrl_schema *, struct rdt_domain *);
    struct list_head evt_list;
    long unsigned int fflags;
    bool cdp_capable;
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
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rdt_resource {
    int rid;
    bool alloc_enabled;
    bool mon_enabled;
    bool alloc_capable;
    bool mon_capable;
    char *name;
    int num_closid;
    int cache_level;
    u32 default_ctrl;
    unsigned int msr_base;
    void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *);
    int data_width;
    struct list_head domains;
    struct rdt_cache cache;
    struct rdt_membw membw;
    const char *format_str;
    int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *);
    bool (*cbm_validate)(char *, u32 *, struct rdt_resource *);
    struct list_head evt_list;
    int num_rmid;
    unsigned int mon_scale;
    long unsigned int fflags;
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
<code>int rid</code>
</li>
<li>
<b>Field added. </b>
<code>bool alloc_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>bool mon_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>bool alloc_capable</code>
</li>
<li>
<b>Field added. </b>
<code>bool mon_capable</code>
</li>
<li>
<b>Field added. </b>
<code>u32 default_ctrl</code>
</li>
<li>
<b>Field added. </b>
<code>void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *)</code>
</li>
<li>
<b>Field added. </b>
<code>int data_width</code>
</li>
<li>
<b>Field added. </b>
<code>struct rdt_cache cache</code>
</li>
<li>
<b>Field added. </b>
<code>struct rdt_membw membw</code>
</li>
<li>
<b>Field added. </b>
<code>const char *format_str</code>
</li>
<li>
<b>Field added. </b>
<code>int (*parse_ctrlval)(char *, struct rdt_resource *, struct rdt_domain *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head evt_list</code>
</li>
<li>
<b>Field added. </b>
<code>int num_rmid</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int mon_scale</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int fflags</code>
</li>
<li>
<b>Field removed. </b>
<code>bool enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>bool capable</code>
</li>
<li>
<b>Field removed. </b>
<code>int cbm_len</code>
</li>
<li>
<b>Field removed. </b>
<code>int min_cbm_bits</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 max_cbm</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_domains</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 *tmp_cbms</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_tmp_cbms</code>
</li>
<li>
<b>Field removed. </b>
<code>int cbm_idx_multi</code>
</li>
<li>
<b>Field removed. </b>
<code>int cbm_idx_offset</code>
</li>
<li>
<b>Field type changed. </b>
<code>int msr_base</code> ➡️ <code>unsigned int msr_base</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*cbm_validate)(char *, u32 *, struct rdt_resource *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*parse_ctrlval)(char *, struct rdt_resource *, struct rdt_domain *)</code> ➡️ <code>int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *)</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int mbm_width</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool (*cbm_validate)(char *, u32 *, struct rdt_resource *)</code>
</li>
</ul>
</details>
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
<code>bool cdp_capable</code>
</li>
<li>
<b>Field removed. </b>
<code>int num_closid</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int msr_base</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*msr_update)(struct rdt_domain *, struct msr_param *, struct rdt_resource *)</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int mon_scale</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int mbm_width</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rdt_cache cache</code> ➡️ <code>struct resctrl_cache cache</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rdt_membw membw</code> ➡️ <code>struct resctrl_membw membw</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*parse_ctrlval)(struct rdt_parse_data *, struct rdt_resource *, struct rdt_domain *)</code> ➡️ <code>int (*parse_ctrlval)(struct rdt_parse_data *, struct resctrl_schema *, struct rdt_domain *)</code>
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
<b>Field removed. </b>
<code>bool alloc_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>bool mon_enabled</code>
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
