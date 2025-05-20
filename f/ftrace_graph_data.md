# Struct: <code>ftrace_graph_data</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ftrace_graph_data {
    long unsigned int *table;
    size_t size;
    int *count;
    const struct seq_operations *seq_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ftrace_graph_data {
    long unsigned int *table;
    size_t size;
    int *count;
    const struct seq_operations *seq_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ftrace_graph_data {
    long unsigned int *table;
    size_t size;
    int *count;
    const struct seq_operations *seq_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
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
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
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
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ftrace_graph_data {
    struct ftrace_hash *hash;
    struct ftrace_func_entry *entry;
    int idx;
    enum graph_filter_type type;
    struct ftrace_hash *new_hash;
    const struct seq_operations *seq_ops;
    struct trace_parser parser;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ftrace_hash *hash</code>
</li>
<li>
<b>Field added. </b>
<code>struct ftrace_func_entry *entry</code>
</li>
<li>
<b>Field added. </b>
<code>int idx</code>
</li>
<li>
<b>Field added. </b>
<code>enum graph_filter_type type</code>
</li>
<li>
<b>Field added. </b>
<code>struct ftrace_hash *new_hash</code>
</li>
<li>
<b>Field added. </b>
<code>struct trace_parser parser</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int *table</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t size</code>
</li>
<li>
<b>Field removed. </b>
<code>int *count</code>
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
