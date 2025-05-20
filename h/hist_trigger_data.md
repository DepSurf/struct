# Struct: <code>hist_trigger_data</code>

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
struct hist_trigger_data {
    struct hist_field * fields[5];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[5];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[5];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[6];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct hist_field * synth_var_refs[16];
    unsigned int n_synth_var_refs;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * max_vars[16];
    unsigned int n_max_vars;
    unsigned int n_max_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * max_vars[16];
    unsigned int n_max_vars;
    unsigned int n_max_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[32];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[32];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[32];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int n_var_str;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[32];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[32];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[32];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int n_var_str;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[32];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[32];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[32];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int n_var_str;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[64];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[64];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[64];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int n_var_str;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[64];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[64];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[64];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int n_var_str;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[64];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[64];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[64];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int n_var_str;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[64];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[64];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[64];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int n_var_str;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[64];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[64];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[64];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
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
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
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
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
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
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hist_trigger_data {
    struct hist_field * fields[22];
    unsigned int n_vals;
    unsigned int n_keys;
    unsigned int n_fields;
    unsigned int n_vars;
    unsigned int key_size;
    struct tracing_map_sort_key sort_keys[2];
    unsigned int n_sort_keys;
    struct trace_event_file *event_file;
    struct hist_trigger_attrs *attrs;
    struct tracing_map *map;
    bool enable_timestamps;
    bool remove;
    struct hist_field * var_refs[16];
    unsigned int n_var_refs;
    struct action_data * actions[8];
    unsigned int n_actions;
    struct field_var * field_vars[16];
    unsigned int n_field_vars;
    unsigned int n_field_var_str;
    struct field_var_hist * field_var_hists[16];
    unsigned int n_field_var_hists;
    struct field_var * save_vars[16];
    unsigned int n_save_vars;
    unsigned int n_save_var_str;
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
<b>Field type changed. </b>
<code>struct hist_field * fields[5]</code> ➡️ <code>struct hist_field * fields[6]</code>
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
<code>unsigned int n_vars</code>
</li>
<li>
<b>Field added. </b>
<code>bool enable_timestamps</code>
</li>
<li>
<b>Field added. </b>
<code>bool remove</code>
</li>
<li>
<b>Field added. </b>
<code>struct hist_field * var_refs[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_var_refs</code>
</li>
<li>
<b>Field added. </b>
<code>struct action_data * actions[8]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_actions</code>
</li>
<li>
<b>Field added. </b>
<code>struct hist_field * synth_var_refs[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_synth_var_refs</code>
</li>
<li>
<b>Field added. </b>
<code>struct field_var * field_vars[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_field_vars</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_field_var_str</code>
</li>
<li>
<b>Field added. </b>
<code>struct field_var_hist * field_var_hists[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_field_var_hists</code>
</li>
<li>
<b>Field added. </b>
<code>struct field_var * max_vars[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_max_vars</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_max_var_str</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct hist_field * fields[6]</code> ➡️ <code>struct hist_field * fields[22]</code>
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
<code>struct hist_field * synth_var_refs[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int n_synth_var_refs</code>
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
<code>struct field_var * save_vars[16]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_save_vars</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int n_save_var_str</code>
</li>
<li>
<b>Field removed. </b>
<code>struct field_var * max_vars[16]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int n_max_vars</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int n_max_var_str</code>
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
<b>Field type changed. </b>
<code>struct field_var * field_vars[16]</code> ➡️ <code>struct field_var * field_vars[32]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct field_var_hist * field_var_hists[16]</code> ➡️ <code>struct field_var_hist * field_var_hists[32]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct field_var * save_vars[16]</code> ➡️ <code>struct field_var * save_vars[32]</code>
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
<code>unsigned int n_var_str</code>
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
<b>Field type changed. </b>
<code>struct field_var * field_vars[32]</code> ➡️ <code>struct field_var * field_vars[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct field_var_hist * field_var_hists[32]</code> ➡️ <code>struct field_var_hist * field_var_hists[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct field_var * save_vars[32]</code> ➡️ <code>struct field_var * save_vars[64]</code>
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
