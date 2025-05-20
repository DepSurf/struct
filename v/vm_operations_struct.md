# Struct: <code>vm_operations_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*mremap)(struct vm_area_struct *);
    int (*fault)(struct vm_area_struct *, struct vm_fault *);
    int (*pmd_fault)(struct vm_area_struct *, long unsigned int, pmd_t *, unsigned int);
    void (*map_pages)(struct vm_area_struct *, struct vm_fault *);
    int (*page_mkwrite)(struct vm_area_struct *, struct vm_fault *);
    int (*pfn_mkwrite)(struct vm_area_struct *, struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*mremap)(struct vm_area_struct *);
    int (*fault)(struct vm_area_struct *, struct vm_fault *);
    int (*pmd_fault)(struct vm_area_struct *, long unsigned int, pmd_t *, unsigned int);
    void (*map_pages)(struct fault_env *, long unsigned int, long unsigned int);
    int (*page_mkwrite)(struct vm_area_struct *, struct vm_fault *);
    int (*pfn_mkwrite)(struct vm_area_struct *, struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*mremap)(struct vm_area_struct *);
    int (*fault)(struct vm_area_struct *, struct vm_fault *);
    int (*pmd_fault)(struct vm_area_struct *, long unsigned int, pmd_t *, unsigned int);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    int (*page_mkwrite)(struct vm_area_struct *, struct vm_fault *);
    int (*pfn_mkwrite)(struct vm_area_struct *, struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*mremap)(struct vm_area_struct *);
    int (*fault)(struct vm_fault *);
    int (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    int (*page_mkwrite)(struct vm_fault *);
    int (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    int (*fault)(struct vm_fault *);
    int (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    int (*page_mkwrite)(struct vm_fault *);
    int (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*may_split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *, long unsigned int);
    int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*may_split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    vm_fault_t (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*may_split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    vm_fault_t (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*may_split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    vm_fault_t (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*may_split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    vm_fault_t (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*may_split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    vm_fault_t (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*may_split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, unsigned int);
    vm_fault_t (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int, long unsigned int *);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
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
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
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
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vm_operations_struct {
    void (*open)(struct vm_area_struct *);
    void (*close)(struct vm_area_struct *);
    int (*split)(struct vm_area_struct *, long unsigned int);
    int (*mremap)(struct vm_area_struct *);
    vm_fault_t (*fault)(struct vm_fault *);
    vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size);
    void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int);
    long unsigned int (*pagesize)(struct vm_area_struct *);
    vm_fault_t (*page_mkwrite)(struct vm_fault *);
    vm_fault_t (*pfn_mkwrite)(struct vm_fault *);
    int (*access)(struct vm_area_struct *, long unsigned int, void *, int, int);
    const char * (*name)(struct vm_area_struct *);
    int (*set_policy)(struct vm_area_struct *, struct mempolicy *);
    struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int);
    struct page * (*find_special_page)(struct vm_area_struct *, long unsigned int);
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
<b>Field type changed. </b>
<code>void (*map_pages)(struct vm_area_struct *, struct vm_fault *)</code> ➡️ <code>void (*map_pages)(struct fault_env *, long unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*map_pages)(struct fault_env *, long unsigned int, long unsigned int)</code> ➡️ <code>void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*huge_fault)(struct vm_fault *, enum page_entry_size)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*pmd_fault)(struct vm_area_struct *, long unsigned int, pmd_t *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*fault)(struct vm_area_struct *, struct vm_fault *)</code> ➡️ <code>int (*fault)(struct vm_fault *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*page_mkwrite)(struct vm_area_struct *, struct vm_fault *)</code> ➡️ <code>int (*page_mkwrite)(struct vm_fault *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*pfn_mkwrite)(struct vm_area_struct *, struct vm_fault *)</code> ➡️ <code>int (*pfn_mkwrite)(struct vm_fault *)</code>
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
<code>int (*split)(struct vm_area_struct *, long unsigned int)</code>
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
<code>long unsigned int (*pagesize)(struct vm_area_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*fault)(struct vm_fault *)</code> ➡️ <code>vm_fault_t (*fault)(struct vm_fault *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*huge_fault)(struct vm_fault *, enum page_entry_size)</code> ➡️ <code>vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*page_mkwrite)(struct vm_fault *)</code> ➡️ <code>vm_fault_t (*page_mkwrite)(struct vm_fault *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*pfn_mkwrite)(struct vm_fault *)</code> ➡️ <code>vm_fault_t (*pfn_mkwrite)(struct vm_fault *)</code>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*may_split)(struct vm_area_struct *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*mprotect)(struct vm_area_struct *, long unsigned int, long unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*split)(struct vm_area_struct *, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*mremap)(struct vm_area_struct *)</code> ➡️ <code>int (*mremap)(struct vm_area_struct *, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*mremap)(struct vm_area_struct *, long unsigned int)</code> ➡️ <code>int (*mremap)(struct vm_area_struct *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int)</code> ➡️ <code>vm_fault_t (*map_pages)(struct vm_fault *, long unsigned int, long unsigned int)</code>
</li>
</ul>
</details>
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>vm_fault_t (*huge_fault)(struct vm_fault *, enum page_entry_size)</code> ➡️ <code>vm_fault_t (*huge_fault)(struct vm_fault *, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int)</code> ➡️ <code>struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int, long unsigned int *)</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*set_policy)(struct vm_area_struct *, struct mempolicy *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*set_policy)(struct vm_area_struct *, struct mempolicy *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct mempolicy * (*get_policy)(struct vm_area_struct *, long unsigned int)</code>
</li>
</ul>
</details>
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
