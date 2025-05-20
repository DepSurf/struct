# Struct: <code>action_data</code>

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
In <code>4.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct action_data {
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    struct (anon) onmatch;
    struct (anon) onmax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct action_data {
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    struct (anon) onmatch;
    struct (anon) onmax;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx;
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[32];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[32];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[32];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[64];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[64];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[64];
    unsigned int var_ref_idx[64];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[64];
    unsigned int var_ref_idx[64];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[64];
    unsigned int var_ref_idx[64];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
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
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
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
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
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
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct action_data {
    enum handler_id handler;
    enum action_id action;
    char *action_name;
    action_fn_t fn;
    unsigned int n_params;
    char * params[16];
    unsigned int var_ref_idx[16];
    struct synth_event *synth_event;
    bool use_trace_keyword;
    char *synth_event_name;
    struct (anon) match_data;
    struct (anon) track_data;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum handler_id handler</code>
</li>
<li>
<b>Field added. </b>
<code>enum action_id action</code>
</li>
<li>
<b>Field added. </b>
<code>char *action_name</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int var_ref_idx</code>
</li>
<li>
<b>Field added. </b>
<code>struct synth_event *synth_event</code>
</li>
<li>
<b>Field added. </b>
<code>bool use_trace_keyword</code>
</li>
<li>
<b>Field added. </b>
<code>char *synth_event_name</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) match_data</code>
</li>
<li>
<b>Field added. </b>
<code>struct (anon) track_data</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) onmatch</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) onmax</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>unsigned int var_ref_idx</code> ➡️ <code>unsigned int var_ref_idx[16]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char * params[16]</code> ➡️ <code>char * params[32]</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>char * params[32]</code> ➡️ <code>char * params[64]</code>
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
<b>Field type changed. </b>
<code>unsigned int var_ref_idx[16]</code> ➡️ <code>unsigned int var_ref_idx[64]</code>
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
