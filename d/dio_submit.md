# Struct: <code>dio_submit</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
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
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
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
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dio_submit {
    struct bio *bio;
    unsigned int blkbits;
    unsigned int blkfactor;
    unsigned int start_zero_done;
    int pages_in_io;
    sector_t block_in_file;
    unsigned int blocks_available;
    int reap_counter;
    sector_t final_block_in_request;
    int boundary;
    get_block_t *get_block;
    dio_submit_t *submit_io;
    loff_t logical_offset_in_bio;
    sector_t final_block_in_bio;
    sector_t next_block_for_io;
    struct page *cur_page;
    unsigned int cur_page_offset;
    unsigned int cur_page_len;
    sector_t cur_page_block;
    loff_t cur_page_fs_offset;
    struct iov_iter *iter;
    unsigned int head;
    unsigned int tail;
    size_t from;
    size_t to;
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
<b>Field removed. </b>
<code>dio_submit_t *submit_io</code>
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
