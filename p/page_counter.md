# Struct: <code>page_counter</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t count;
    long unsigned int limit;
    struct page_counter *parent;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t count;
    long unsigned int limit;
    struct page_counter *parent;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t count;
    long unsigned int limit;
    struct page_counter *parent;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t count;
    long unsigned int limit;
    struct page_counter *parent;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t count;
    long unsigned int limit;
    struct page_counter *parent;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
    struct page_counter *parent;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
    struct page_counter *parent;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
    struct page_counter *parent;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    struct cacheline_padding _pad1_;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
    struct cacheline_padding _pad2_;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    struct page_counter *parent;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    struct cacheline_padding _pad1_;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
    struct cacheline_padding _pad2_;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    struct page_counter *parent;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    struct cacheline_padding _pad1_;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
    struct cacheline_padding _pad2_;
    long unsigned int min;
    long unsigned int low;
    long unsigned int high;
    long unsigned int max;
    struct page_counter *parent;
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
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
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
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct page_counter {
    atomic_long_t usage;
    long unsigned int min;
    long unsigned int low;
    long unsigned int max;
    struct page_counter *parent;
    long unsigned int emin;
    atomic_long_t min_usage;
    atomic_long_t children_min_usage;
    long unsigned int elow;
    atomic_long_t low_usage;
    atomic_long_t children_low_usage;
    long unsigned int watermark;
    long unsigned int failcnt;
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
<b>Field added. </b>
<code>atomic_long_t usage</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int min</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int low</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int max</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int emin</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t min_usage</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t children_min_usage</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int elow</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t low_usage</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t children_low_usage</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_long_t count</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int limit</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int high</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cacheline_padding _pad1_</code>
</li>
<li>
<b>Field added. </b>
<code>struct cacheline_padding _pad2_</code>
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
