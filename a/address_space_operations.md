# Struct: <code>address_space_operations</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *, loff_t);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*read_folio)(struct file *, struct folio *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    bool (*dirty_folio)(struct address_space *, struct folio *);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidate_folio)(struct folio *, size_t, size_t);
    bool (*release_folio)(struct folio *, gfp_t);
    void (*free_folio)(struct folio *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_folio)(struct folio *);
    bool (*is_partially_uptodate)(struct folio *, size_t, size_t);
    void (*is_dirty_writeback)(struct folio *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
    int (*swap_rw)(struct kiocb *, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*read_folio)(struct file *, struct folio *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    bool (*dirty_folio)(struct address_space *, struct folio *);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidate_folio)(struct folio *, size_t, size_t);
    bool (*release_folio)(struct folio *, gfp_t);
    void (*free_folio)(struct folio *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migrate_folio)(struct address_space *, struct folio *, struct folio *, enum migrate_mode);
    int (*launder_folio)(struct folio *);
    bool (*is_partially_uptodate)(struct folio *, size_t, size_t);
    void (*is_dirty_writeback)(struct folio *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
    int (*swap_rw)(struct kiocb *, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*read_folio)(struct file *, struct folio *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    bool (*dirty_folio)(struct address_space *, struct folio *);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidate_folio)(struct folio *, size_t, size_t);
    bool (*release_folio)(struct folio *, gfp_t);
    void (*free_folio)(struct folio *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migrate_folio)(struct address_space *, struct folio *, struct folio *, enum migrate_mode);
    int (*launder_folio)(struct folio *);
    bool (*is_partially_uptodate)(struct folio *, size_t, size_t);
    void (*is_dirty_writeback)(struct folio *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
    int (*swap_rw)(struct kiocb *, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*read_folio)(struct file *, struct folio *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    bool (*dirty_folio)(struct address_space *, struct folio *);
    void (*readahead)(struct readahead_control *);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidate_folio)(struct folio *, size_t, size_t);
    bool (*release_folio)(struct folio *, gfp_t);
    void (*free_folio)(struct folio *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migrate_folio)(struct address_space *, struct folio *, struct folio *, enum migrate_mode);
    int (*launder_folio)(struct folio *);
    bool (*is_partially_uptodate)(struct folio *, size_t, size_t);
    void (*is_dirty_writeback)(struct folio *, bool *, bool *);
    int (*error_remove_folio)(struct address_space *, struct folio *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
    int (*swap_rw)(struct kiocb *, struct iov_iter *);
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
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
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
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct address_space_operations {
    int (*writepage)(struct page *, struct writeback_control *);
    int (*readpage)(struct file *, struct page *);
    int (*writepages)(struct address_space *, struct writeback_control *);
    int (*set_page_dirty)(struct page *);
    int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int);
    int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **);
    int (*write_end)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page *, void *);
    sector_t (*bmap)(struct address_space *, sector_t);
    void (*invalidatepage)(struct page *, unsigned int, unsigned int);
    int (*releasepage)(struct page *, gfp_t);
    void (*freepage)(struct page *);
    ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *);
    int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode);
    bool (*isolate_page)(struct page *, isolate_mode_t);
    void (*putback_page)(struct page *);
    int (*launder_page)(struct page *);
    int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int);
    void (*is_dirty_writeback)(struct page *, bool *, bool *);
    int (*error_remove_page)(struct address_space *, struct page *);
    int (*swap_activate)(struct swap_info_struct *, struct file *, sector_t *);
    void (*swap_deactivate)(struct file *);
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
<code>bool (*isolate_page)(struct page *, isolate_mode_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*putback_page)(struct page *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *, loff_t)</code> ➡️ <code>ssize_t (*direct_IO)(struct kiocb *, struct iov_iter *)</code>
</li>
</ul>
</details>
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
<code>void (*readahead)(struct readahead_control *)</code>
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
<code>int (*read_folio)(struct file *, struct folio *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*dirty_folio)(struct address_space *, struct folio *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*invalidate_folio)(struct folio *, size_t, size_t)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*release_folio)(struct folio *, gfp_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*free_folio)(struct folio *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*launder_folio)(struct folio *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*swap_rw)(struct kiocb *, struct iov_iter *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*readpage)(struct file *, struct page *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_page_dirty)(struct page *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*readpages)(struct file *, struct address_space *, struct list_head *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*invalidatepage)(struct page *, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*releasepage)(struct page *, gfp_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*freepage)(struct page *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*launder_page)(struct page *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, unsigned int, struct page **, void **)</code> ➡️ <code>int (*write_begin)(struct file *, struct address_space *, loff_t, unsigned int, struct page **, void **)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*is_partially_uptodate)(struct page *, long unsigned int, long unsigned int)</code> ➡️ <code>bool (*is_partially_uptodate)(struct folio *, size_t, size_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*is_dirty_writeback)(struct page *, bool *, bool *)</code> ➡️ <code>void (*is_dirty_writeback)(struct folio *, bool *, bool *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*migrate_folio)(struct address_space *, struct folio *, struct folio *, enum migrate_mode)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*migratepage)(struct address_space *, struct page *, struct page *, enum migrate_mode)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*isolate_page)(struct page *, isolate_mode_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*putback_page)(struct page *)</code>
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
<code>int (*error_remove_folio)(struct address_space *, struct folio *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*error_remove_page)(struct address_space *, struct page *)</code>
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
