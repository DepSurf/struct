# Struct: <code>dma_fence_ops</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dma_fence_ops {
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    int (*fill_driver_data)(struct dma_fence *, void *, int);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dma_fence_ops {
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    int (*fill_driver_data)(struct dma_fence *, void *, int);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dma_fence_ops {
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    int (*fill_driver_data)(struct dma_fence *, void *, int);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dma_fence_ops {
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    int (*fill_driver_data)(struct dma_fence *, void *, int);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dma_fence_ops {
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
    void (*set_deadline)(struct dma_fence *, ktime_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
    void (*set_deadline)(struct dma_fence *, ktime_t);
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
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
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
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dma_fence_ops {
    bool use_64bit_seqno;
    const char * (*get_driver_name)(struct dma_fence *);
    const char * (*get_timeline_name)(struct dma_fence *);
    bool (*enable_signaling)(struct dma_fence *);
    bool (*signaled)(struct dma_fence *);
    long int (*wait)(struct dma_fence *, bool, long int);
    void (*release)(struct dma_fence *);
    void (*fence_value_str)(struct dma_fence *, char *, int);
    void (*timeline_value_str)(struct dma_fence *, char *, int);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*fill_driver_data)(struct dma_fence *, void *, int)</code>
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
<code>bool use_64bit_seqno</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*set_deadline)(struct dma_fence *, ktime_t)</code>
</li>
</ul>
</details>
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
