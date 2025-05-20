# Struct: <code>cpuhp_cpu_state</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    enum cpuhp_state cb_state;
    int (*cb)(unsigned int);
    int result;
    struct completion done;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    enum cpuhp_state cb_state;
    int result;
    struct completion done;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    enum cpuhp_state cb_state;
    int result;
    struct completion done;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    bool booted_once;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    bool booted_once;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    bool booted_once;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    int cpu;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    int cpu;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    atomic_t ap_sync_state;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    atomic_t ap_sync_state;
    struct completion done_up;
    struct completion done_down;
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
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
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
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpuhp_cpu_state {
    enum cpuhp_state state;
    enum cpuhp_state target;
    enum cpuhp_state fail;
    struct task_struct *thread;
    bool should_run;
    bool rollback;
    bool single;
    bool bringup;
    struct hlist_node *node;
    struct hlist_node *last;
    enum cpuhp_state cb_state;
    int result;
    struct completion done_up;
    struct completion done_down;
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
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool single</code>
</li>
<li>
<b>Field added. </b>
<code>bool bringup</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node *node</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*cb)(unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum cpuhp_state fail</code>
</li>
<li>
<b>Field added. </b>
<code>struct hlist_node *last</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion done_up</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion done_down</code>
</li>
<li>
<b>Field removed. </b>
<code>struct completion done</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool booted_once</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
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
<code>bool booted_once</code>
</li>
</ul>
</details>
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
<code>int cpu</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int cpu</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_t ap_sync_state</code>
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
