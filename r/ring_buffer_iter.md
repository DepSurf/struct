# Struct: <code>ring_buffer_iter</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    int missed_events;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    int missed_events;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    int missed_events;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    int missed_events;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    int missed_events;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    int missed_events;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    long unsigned int cache_pages_removed;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    int missed_events;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    long unsigned int next_event;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    long unsigned int cache_pages_removed;
    u64 read_stamp;
    u64 page_stamp;
    struct ring_buffer_event *event;
    size_t event_size;
    int missed_events;
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
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
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
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ring_buffer_iter {
    struct ring_buffer_per_cpu *cpu_buffer;
    long unsigned int head;
    struct buffer_page *head_page;
    struct buffer_page *cache_reader_page;
    long unsigned int cache_read;
    u64 read_stamp;
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
<code>long unsigned int next_event</code>
</li>
<li>
<b>Field added. </b>
<code>u64 page_stamp</code>
</li>
<li>
<b>Field added. </b>
<code>struct ring_buffer_event *event</code>
</li>
<li>
<b>Field added. </b>
<code>int missed_events</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int cache_pages_removed</code>
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
<code>size_t event_size</code>
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
