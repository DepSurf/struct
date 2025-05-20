# Struct: <code>iomap_ioend</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    void *io_private;
    struct bio *io_bio;
    struct bio io_inline_bio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    void *io_private;
    struct bio *io_bio;
    struct bio io_inline_bio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    struct bio *io_bio;
    struct bio io_inline_bio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    struct bio *io_bio;
    struct bio io_inline_bio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    u32 io_folios;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    sector_t io_sector;
    struct bio *io_bio;
    struct bio io_inline_bio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    u32 io_folios;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    sector_t io_sector;
    struct bio *io_bio;
    struct bio io_inline_bio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    u32 io_folios;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    sector_t io_sector;
    struct bio *io_bio;
    struct bio io_inline_bio;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct iomap_ioend {
    struct list_head io_list;
    u16 io_type;
    u16 io_flags;
    u32 io_folios;
    struct inode *io_inode;
    size_t io_size;
    loff_t io_offset;
    sector_t io_sector;
    struct bio *io_bio;
    struct bio io_inline_bio;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void *io_private</code>
</li>
</ul>
</details>
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
<code>u32 io_folios</code>
</li>
<li>
<b>Field added. </b>
<code>sector_t io_sector</code>
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
