# Struct: <code>dax_operations</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    void (*flush)(struct dax_device *, long unsigned int, void *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, enum dax_access_mode, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
    size_t (*recovery_write)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, enum dax_access_mode, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
    size_t (*recovery_write)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, enum dax_access_mode, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
    size_t (*recovery_write)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, enum dax_access_mode, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    int (*zero_page_range)(struct dax_device *, long unsigned int, size_t);
    size_t (*recovery_write)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
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
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
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
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dax_operations {
    long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *);
    bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t);
    size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
    size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *);
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
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*flush)(struct dax_device *, long unsigned int, void *, size_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*dax_supported)(struct dax_device *, struct block_device *, int, sector_t, sector_t)</code>
</li>
</ul>
</details>
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
<code>int (*zero_page_range)(struct dax_device *, long unsigned int, size_t)</code>
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
<code>size_t (*recovery_write)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *)</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t (*copy_from_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *)</code>
</li>
<li>
<b>Field removed. </b>
<code>size_t (*copy_to_iter)(struct dax_device *, long unsigned int, void *, size_t, struct iov_iter *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int (*direct_access)(struct dax_device *, long unsigned int, long int, void **, pfn_t *)</code> ➡️ <code>long int (*direct_access)(struct dax_device *, long unsigned int, long int, enum dax_access_mode, void **, pfn_t *)</code>
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
