# Struct: <code>iomap</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct iomap {
    sector_t blkno;
    loff_t offset;
    u64 length;
    int type;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct iomap {
    sector_t blkno;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct iomap {
    sector_t blkno;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct iomap {
    sector_t blkno;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    void (*page_done)(struct inode *, loff_t, unsigned int, struct page *, struct iomap *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
    u64 validity_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_folio_ops *folio_ops;
    u64 validity_cookie;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_folio_ops *folio_ops;
    u64 validity_cookie;
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
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
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
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct iomap {
    u64 addr;
    loff_t offset;
    u64 length;
    u16 type;
    u16 flags;
    struct block_device *bdev;
    struct dax_device *dax_dev;
    void *inline_data;
    void *private;
    const struct iomap_page_ops *page_ops;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 flags</code>
</li>
<li>
<b>Field added. </b>
<code>struct block_device *bdev</code>
</li>
<li>
<b>Field type changed. </b>
<code>int type</code> ➡️ <code>u16 type</code>
</li>
</ul>
</details>
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
<code>struct dax_device *dax_dev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 addr</code>
</li>
<li>
<b>Field removed. </b>
<code>sector_t blkno</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *inline_data</code>
</li>
<li>
<b>Field added. </b>
<code>void *private</code>
</li>
<li>
<b>Field added. </b>
<code>void (*page_done)(struct inode *, loff_t, unsigned int, struct page *, struct iomap *)</code>
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
<code>const struct iomap_page_ops *page_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*page_done)(struct inode *, loff_t, unsigned int, struct page *, struct iomap *)</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 validity_cookie</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const struct iomap_folio_ops *folio_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct iomap_page_ops *page_ops</code>
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
