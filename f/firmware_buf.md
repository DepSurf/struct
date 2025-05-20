# Struct: <code>firmware_buf</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct firmware_buf {
    struct kref ref;
    struct list_head list;
    struct completion completion;
    struct firmware_cache *fwc;
    long unsigned int status;
    void *data;
    size_t size;
    bool is_paged_buf;
    bool need_uevent;
    struct page **pages;
    int nr_pages;
    int page_array_size;
    struct list_head pending_list;
    const char *fw_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct firmware_buf {
    struct kref ref;
    struct list_head list;
    struct completion completion;
    struct firmware_cache *fwc;
    long unsigned int status;
    void *data;
    size_t size;
    size_t allocated_size;
    bool is_paged_buf;
    bool need_uevent;
    struct page **pages;
    int nr_pages;
    int page_array_size;
    struct list_head pending_list;
    const char *fw_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct firmware_buf {
    struct kref ref;
    struct list_head list;
    struct firmware_cache *fwc;
    struct fw_state fw_st;
    void *data;
    size_t size;
    size_t allocated_size;
    bool is_paged_buf;
    bool need_uevent;
    struct page **pages;
    int nr_pages;
    int page_array_size;
    struct list_head pending_list;
    const char *fw_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct firmware_buf {
    struct kref ref;
    struct list_head list;
    struct firmware_cache *fwc;
    struct fw_state fw_st;
    void *data;
    size_t size;
    size_t allocated_size;
    bool is_paged_buf;
    bool need_uevent;
    struct page **pages;
    int nr_pages;
    int page_array_size;
    struct list_head pending_list;
    const char *fw_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct firmware_buf {
    struct kref ref;
    struct list_head list;
    struct firmware_cache *fwc;
    struct fw_state fw_st;
    void *data;
    size_t size;
    size_t allocated_size;
    bool is_paged_buf;
    bool need_uevent;
    struct page **pages;
    int nr_pages;
    int page_array_size;
    struct list_head pending_list;
    const char *fw_id;
};
```
</details>
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
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
<details>
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t allocated_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct fw_state fw_st</code>
</li>
<li>
<b>Field removed. </b>
<code>struct completion completion</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int status</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
</ul>
