# Struct: <code>event_command</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    bool post_trigger;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*parse)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*parse)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*parse)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*parse)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
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
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
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
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct event_command {
    struct list_head list;
    char *name;
    enum event_trigger_type trigger_type;
    int flags;
    int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *);
    int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *);
    void (*unreg_all)(struct trace_event_file *);
    int (*set_filter)(char *, struct event_trigger_data *, struct trace_event_file *);
    struct event_trigger_ops * (*get_trigger_ops)(char *, char *);
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
<code>int flags</code>
</li>
<li>
<b>Field added. </b>
<code>void (*unreg_all)(struct trace_event_file *)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool post_trigger</code>
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
<code>int (*parse)(struct event_command *, struct trace_event_file *, char *, char *, char *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*func)(struct event_command *, struct trace_event_file *, char *, char *, char *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*reg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *)</code> ➡️ <code>int (*reg)(char *, struct event_trigger_data *, struct trace_event_file *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*unreg)(char *, struct event_trigger_ops *, struct event_trigger_data *, struct trace_event_file *)</code> ➡️ <code>void (*unreg)(char *, struct event_trigger_data *, struct trace_event_file *)</code>
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
