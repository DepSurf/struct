# Struct: <code>filter_pred</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
    short unsigned int index;
    short unsigned int parent;
    short unsigned int left;
    short unsigned int right;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
    short unsigned int index;
    short unsigned int parent;
    short unsigned int left;
    short unsigned int right;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
    short unsigned int index;
    short unsigned int parent;
    short unsigned int left;
    short unsigned int right;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
    short unsigned int index;
    short unsigned int parent;
    short unsigned int left;
    short unsigned int right;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
    short unsigned int index;
    short unsigned int parent;
    short unsigned int left;
    short unsigned int right;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct filter_pred {
    enum filter_pred_fn fn_num;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct filter_pred {
    enum filter_pred_fn fn_num;
    u64 val;
    u64 val2;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct filter_pred {
    struct regex *regex;
    struct cpumask *mask;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    u64 val;
    u64 val2;
    enum filter_pred_fn fn_num;
    int offset;
    int not;
    int op;
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
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
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
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct filter_pred {
    filter_pred_fn_t fn;
    u64 val;
    struct regex regex;
    short unsigned int *ops;
    struct ftrace_event_field *field;
    int offset;
    int not;
    int op;
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
<b>Field removed. </b>
<code>short unsigned int index</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int parent</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int left</code>
</li>
<li>
<b>Field removed. </b>
<code>short unsigned int right</code>
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
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum filter_pred_fn fn_num</code>
</li>
<li>
<b>Field removed. </b>
<code>filter_pred_fn_t fn</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 val2</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cpumask *mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct regex regex</code> ➡️ <code>struct regex *regex</code>
</li>
</ul>
</details>
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
