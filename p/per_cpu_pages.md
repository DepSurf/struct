# Struct: <code>per_cpu_pages</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    short int free_factor;
    short int expire;
    struct list_head lists[15];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    short int free_factor;
    short int expire;
    struct list_head lists[15];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct per_cpu_pages {
    spinlock_t lock;
    int count;
    int high;
    int batch;
    short int free_factor;
    short int expire;
    struct list_head lists[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct per_cpu_pages {
    spinlock_t lock;
    int count;
    int high;
    int batch;
    short int free_factor;
    short int expire;
    struct list_head lists[13];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct per_cpu_pages {
    spinlock_t lock;
    int count;
    int high;
    int high_min;
    int high_max;
    int batch;
    u8 flags;
    u8 alloc_factor;
    u8 expire;
    short int free_count;
    struct list_head lists[13];
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
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
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
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct per_cpu_pages {
    int count;
    int high;
    int batch;
    struct list_head lists[3];
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
<b>Field added. </b>
<code>short int free_factor</code>
</li>
<li>
<b>Field added. </b>
<code>short int expire</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head lists[3]</code> ➡️ <code>struct list_head lists[15]</code>
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
<b>Field added. </b>
<code>spinlock_t lock</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct list_head lists[15]</code> ➡️ <code>struct list_head lists[13]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int high_min</code>
</li>
<li>
<b>Field added. </b>
<code>int high_max</code>
</li>
<li>
<b>Field added. </b>
<code>u8 flags</code>
</li>
<li>
<b>Field added. </b>
<code>u8 alloc_factor</code>
</li>
<li>
<b>Field added. </b>
<code>short int free_count</code>
</li>
<li>
<b>Field removed. </b>
<code>short int free_factor</code>
</li>
<li>
<b>Field type changed. </b>
<code>short int expire</code> ➡️ <code>u8 expire</code>
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
