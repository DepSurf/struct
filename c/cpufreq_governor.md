# Struct: <code>cpufreq_governor</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int initialized;
    int (*governor)(struct cpufreq_policy *, unsigned int);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    unsigned int max_transition_latency;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    unsigned int max_transition_latency;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    unsigned int max_transition_latency;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    unsigned int max_transition_latency;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    struct list_head governor_list;
    struct module *owner;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    struct list_head governor_list;
    struct module *owner;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    struct list_head governor_list;
    struct module *owner;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    struct list_head governor_list;
    struct module *owner;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    struct list_head governor_list;
    struct module *owner;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    struct list_head governor_list;
    struct module *owner;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    struct list_head governor_list;
    struct module *owner;
    u8 flags;
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
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
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
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpufreq_governor {
    char name[16];
    int (*init)(struct cpufreq_policy *);
    void (*exit)(struct cpufreq_policy *);
    int (*start)(struct cpufreq_policy *);
    void (*stop)(struct cpufreq_policy *);
    void (*limits)(struct cpufreq_policy *);
    ssize_t (*show_setspeed)(struct cpufreq_policy *, char *);
    int (*store_setspeed)(struct cpufreq_policy *, unsigned int);
    bool dynamic_switching;
    struct list_head governor_list;
    struct module *owner;
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
<code>int (*init)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*exit)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*start)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*stop)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*limits)(struct cpufreq_policy *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*governor)(struct cpufreq_policy *, unsigned int)</code>
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
<b>Field added. </b>
<code>bool dynamic_switching</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int max_transition_latency</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 flags</code>
</li>
<li>
<b>Field removed. </b>
<code>bool dynamic_switching</code>
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
