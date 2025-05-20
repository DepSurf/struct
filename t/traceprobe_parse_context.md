# Struct: <code>traceprobe_parse_context</code>

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
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct traceprobe_parse_context {
    struct trace_event_call *event;
    const struct btf_param *params;
    s32 nr_params;
    const char *funcname;
    unsigned int flags;
    int offset;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct traceprobe_parse_context {
    struct trace_event_call *event;
    const char *funcname;
    const struct btf_type *proto;
    const struct btf_param *params;
    s32 nr_params;
    struct btf *btf;
    const struct btf_type *last_type;
    u32 last_bitoffs;
    u32 last_bitsize;
    unsigned int flags;
    int offset;
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct btf_type *proto</code>
</li>
<li>
<b>Field added. </b>
<code>struct btf *btf</code>
</li>
<li>
<b>Field added. </b>
<code>const struct btf_type *last_type</code>
</li>
<li>
<b>Field added. </b>
<code>u32 last_bitoffs</code>
</li>
<li>
<b>Field added. </b>
<code>u32 last_bitsize</code>
</li>
</ul>
</details>
</li>
</ul>
