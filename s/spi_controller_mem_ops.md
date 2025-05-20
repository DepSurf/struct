# Struct: <code>spi_controller_mem_ops</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
    int (*poll_status)(struct spi_mem *, const struct spi_mem_op *, u16, u16, long unsigned int, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
    int (*poll_status)(struct spi_mem *, const struct spi_mem_op *, u16, u16, long unsigned int, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
    int (*poll_status)(struct spi_mem *, const struct spi_mem_op *, u16, u16, long unsigned int, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
    int (*poll_status)(struct spi_mem *, const struct spi_mem_op *, u16, u16, long unsigned int, long unsigned int, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
    int (*poll_status)(struct spi_mem *, const struct spi_mem_op *, u16, u16, long unsigned int, long unsigned int, long unsigned int);
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
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
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
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct spi_controller_mem_ops {
    int (*adjust_op_size)(struct spi_mem *, struct spi_mem_op *);
    bool (*supports_op)(struct spi_mem *, const struct spi_mem_op *);
    int (*exec_op)(struct spi_mem *, const struct spi_mem_op *);
    const char * (*get_name)(struct spi_mem *);
    int (*dirmap_create)(struct spi_mem_dirmap_desc *);
    void (*dirmap_destroy)(struct spi_mem_dirmap_desc *);
    ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *);
    ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *);
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
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const char * (*get_name)(struct spi_mem *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dirmap_create)(struct spi_mem_dirmap_desc *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*dirmap_destroy)(struct spi_mem_dirmap_desc *)</code>
</li>
<li>
<b>Field added. </b>
<code>ssize_t (*dirmap_read)(struct spi_mem_dirmap_desc *, u64, size_t, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>ssize_t (*dirmap_write)(struct spi_mem_dirmap_desc *, u64, size_t, const void *)</code>
</li>
</ul>
</details>
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
<code>int (*poll_status)(struct spi_mem *, const struct spi_mem_op *, u16, u16, long unsigned int, long unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
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
