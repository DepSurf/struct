# Struct: <code>iomap_readpage_ctx</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct folio *cur_folio;
    bool cur_folio_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct folio *cur_folio;
    bool cur_folio_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct folio *cur_folio;
    bool cur_folio_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct folio *cur_folio;
    bool cur_folio_in_bio;
    struct bio *bio;
    struct readahead_control *rac;
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
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
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
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iomap_readpage_ctx {
    struct page *cur_page;
    bool cur_page_in_bio;
    bool is_readahead;
    struct bio *bio;
    struct list_head *pages;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>struct readahead_control *rac</code>
</li>
<li>
<b>Field removed. </b>
<code>bool is_readahead</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head *pages</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct folio *cur_folio</code>
</li>
<li>
<b>Field added. </b>
<code>bool cur_folio_in_bio</code>
</li>
<li>
<b>Field removed. </b>
<code>struct page *cur_page</code>
</li>
<li>
<b>Field removed. </b>
<code>bool cur_page_in_bio</code>
</li>
</ul>
</details>
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
