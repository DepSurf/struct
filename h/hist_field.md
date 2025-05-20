# Struct: <code>hist_field</code>

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
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int size;
    unsigned int offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int size;
    unsigned int offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int size;
    unsigned int offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    struct hist_field * operands[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_idx;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
    unsigned int var_str_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
    unsigned int var_str_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    long unsigned int buckets;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
    unsigned int var_str_idx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    long unsigned int buckets;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
    unsigned int var_str_idx;
    u64 constant;
    u64 div_multiplier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    long unsigned int buckets;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    enum hist_field_fn fn_num;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
    unsigned int var_str_idx;
    u64 constant;
    u64 div_multiplier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    long unsigned int buckets;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    enum hist_field_fn fn_num;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
    unsigned int var_str_idx;
    u64 constant;
    u64 div_multiplier;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    long unsigned int buckets;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    enum hist_field_fn fn_num;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
    unsigned int var_str_idx;
    u64 constant;
    u64 div_multiplier;
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
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
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
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hist_field {
    struct ftrace_event_field *field;
    long unsigned int flags;
    hist_field_fn_t fn;
    unsigned int ref;
    unsigned int size;
    unsigned int offset;
    unsigned int is_signed;
    const char *type;
    struct hist_field * operands[2];
    struct hist_trigger_data *hist_data;
    struct hist_var var;
    enum field_op_id operator;
    char *system;
    char *event_name;
    char *name;
    unsigned int var_ref_idx;
    bool read_once;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>unsigned int is_signed</code>
</li>
<li>
<b>Field added. </b>
<code>struct hist_field * operands[2]</code>
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
<code>const char *type</code>
</li>
<li>
<b>Field added. </b>
<code>struct hist_trigger_data *hist_data</code>
</li>
<li>
<b>Field added. </b>
<code>struct hist_var var</code>
</li>
<li>
<b>Field added. </b>
<code>enum field_op_id operator</code>
</li>
<li>
<b>Field added. </b>
<code>char *system</code>
</li>
<li>
<b>Field added. </b>
<code>char *event_name</code>
</li>
<li>
<b>Field added. </b>
<code>char *name</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int var_idx</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int var_ref_idx</code>
</li>
<li>
<b>Field added. </b>
<code>bool read_once</code>
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
<code>unsigned int var_idx</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int ref</code>
</li>
</ul>
</details>
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
<code>unsigned int var_str_idx</code>
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
<code>long unsigned int buckets</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 constant</code>
</li>
<li>
<b>Field added. </b>
<code>u64 div_multiplier</code>
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
<code>enum hist_field_fn fn_num</code>
</li>
<li>
<b>Field removed. </b>
<code>hist_field_fn_t fn</code>
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
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
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
