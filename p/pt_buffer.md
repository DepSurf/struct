# Struct: <code>pt_buffer</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local_t lost;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local_t lost;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local_t lost;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pt_buffer {
    int cpu;
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long unsigned int stop_pos;
    long unsigned int intr_pos;
    void **data_pages;
    struct topa_entry * topa_index[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    bool single;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pt_buffer {
    struct list_head tables;
    struct topa *first;
    struct topa *last;
    struct topa *cur;
    unsigned int cur_idx;
    size_t output_off;
    long unsigned int nr_pages;
    local_t data_size;
    local64_t head;
    bool snapshot;
    long int stop_pos;
    long int intr_pos;
    struct topa_entry *stop_te;
    struct topa_entry *intr_te;
    void **data_pages;
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
<b>Field removed. </b>
<code>local_t lost</code>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct topa_entry *stop_te</code>
</li>
<li>
<b>Field added. </b>
<code>struct topa_entry *intr_te</code>
</li>
<li>
<b>Field removed. </b>
<code>int cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct topa_entry * topa_index[0]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int stop_pos</code> ➡️ <code>long int stop_pos</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int intr_pos</code> ➡️ <code>long int intr_pos</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool single</code>
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
