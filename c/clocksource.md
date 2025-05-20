# Struct: <code>clocksource</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct clocksource {
    cycle_t (*read)(struct clocksource *);
    cycle_t mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    struct list_head wd_list;
    cycle_t cs_last;
    cycle_t wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct clocksource {
    cycle_t (*read)(struct clocksource *);
    cycle_t mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    struct list_head wd_list;
    cycle_t cs_last;
    cycle_t wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum clocksource_ids id;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u32 uncertainty_margin;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum clocksource_ids id;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u32 uncertainty_margin;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum clocksource_ids id;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u32 uncertainty_margin;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum clocksource_ids id;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u32 uncertainty_margin;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum clocksource_ids id;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u32 uncertainty_margin;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    enum clocksource_ids id;
    enum vdso_clock_mode vdso_clock_mode;
    long unsigned int flags;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
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
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
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
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct clocksource {
    u64 (*read)(struct clocksource *);
    u64 mask;
    u32 mult;
    u32 shift;
    u64 max_idle_ns;
    u32 maxadj;
    struct arch_clocksource_data archdata;
    u64 max_cycles;
    const char *name;
    struct list_head list;
    int rating;
    int (*enable)(struct clocksource *);
    void (*disable)(struct clocksource *);
    long unsigned int flags;
    void (*suspend)(struct clocksource *);
    void (*resume)(struct clocksource *);
    void (*mark_unstable)(struct clocksource *);
    void (*tick_stable)(struct clocksource *);
    struct list_head wd_list;
    u64 cs_last;
    u64 wd_last;
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>cycle_t (*read)(struct clocksource *)</code> ➡️ <code>u64 (*read)(struct clocksource *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>cycle_t mask</code> ➡️ <code>u64 mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>cycle_t cs_last</code> ➡️ <code>u64 cs_last</code>
</li>
<li>
<b>Field type changed. </b>
<code>cycle_t wd_last</code> ➡️ <code>u64 wd_last</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*mark_unstable)(struct clocksource *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*tick_stable)(struct clocksource *)</code>
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
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
<code>enum vdso_clock_mode vdso_clock_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>struct arch_clocksource_data archdata</code>
</li>
</ul>
</details>
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
<code>enum clocksource_ids id</code>
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
<code>u32 uncertainty_margin</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head wd_list</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 cs_last</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 wd_last</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct list_head wd_list</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 cs_last</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 wd_last</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct arch_clocksource_data archdata</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head wd_list</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 cs_last</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 wd_last</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct arch_clocksource_data archdata</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head wd_list</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 cs_last</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 wd_last</code>
</li>
</ul>
</details>
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
