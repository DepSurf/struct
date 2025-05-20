# Struct: <code>hstate</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[64];
    unsigned int nr_huge_pages_node[64];
    unsigned int free_huge_pages_node[64];
    unsigned int surplus_huge_pages_node[64];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[64];
    unsigned int nr_huge_pages_node[64];
    unsigned int free_huge_pages_node[64];
    unsigned int surplus_huge_pages_node[64];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files_dfl[7];
    struct cftype cgroup_files_legacy[9];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files_dfl[7];
    struct cftype cgroup_files_legacy[9];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hstate {
    struct mutex resize_lock;
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files_dfl[7];
    struct cftype cgroup_files_legacy[9];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hstate {
    struct mutex resize_lock;
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    unsigned int nr_free_vmemmap_pages;
    struct cftype cgroup_files_dfl[7];
    struct cftype cgroup_files_legacy[9];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hstate {
    struct mutex resize_lock;
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    unsigned int demote_order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int max_huge_pages_node[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    unsigned int optimize_vmemmap_pages;
    struct cftype cgroup_files_dfl[8];
    struct cftype cgroup_files_legacy[10];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hstate {
    struct mutex resize_lock;
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    unsigned int demote_order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int max_huge_pages_node[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files_dfl[8];
    struct cftype cgroup_files_legacy[10];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hstate {
    struct mutex resize_lock;
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    unsigned int demote_order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int max_huge_pages_node[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files_dfl[8];
    struct cftype cgroup_files_legacy[10];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hstate {
    struct mutex resize_lock;
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    unsigned int demote_order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int max_huge_pages_node[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files_dfl[8];
    struct cftype cgroup_files_legacy[10];
    char name[32];
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
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[64];
    unsigned int nr_huge_pages_node[64];
    unsigned int free_huge_pages_node[64];
    unsigned int surplus_huge_pages_node[64];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct hstate {
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[256];
    unsigned int nr_huge_pages_node[256];
    unsigned int free_huge_pages_node[256];
    unsigned int surplus_huge_pages_node[256];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1];
    unsigned int nr_huge_pages_node[1];
    unsigned int free_huge_pages_node[1];
    unsigned int surplus_huge_pages_node[1];
    struct cftype cgroup_files[5];
    char name[32];
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
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hstate {
    int next_nid_to_alloc;
    int next_nid_to_free;
    unsigned int order;
    long unsigned int mask;
    long unsigned int max_huge_pages;
    long unsigned int nr_huge_pages;
    long unsigned int free_huge_pages;
    long unsigned int resv_huge_pages;
    long unsigned int surplus_huge_pages;
    long unsigned int nr_overcommit_huge_pages;
    struct list_head hugepage_activelist;
    struct list_head hugepage_freelists[1024];
    unsigned int nr_huge_pages_node[1024];
    unsigned int free_huge_pages_node[1024];
    unsigned int surplus_huge_pages_node[1024];
    struct cftype cgroup_files[5];
    char name[32];
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct list_head hugepage_freelists[64]</code> ➡️ <code>struct list_head hugepage_freelists[1024]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int nr_huge_pages_node[64]</code> ➡️ <code>unsigned int nr_huge_pages_node[1024]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int free_huge_pages_node[64]</code> ➡️ <code>unsigned int free_huge_pages_node[1024]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int surplus_huge_pages_node[64]</code> ➡️ <code>unsigned int surplus_huge_pages_node[1024]</code>
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
<code>struct cftype cgroup_files_dfl[7]</code>
</li>
<li>
<b>Field added. </b>
<code>struct cftype cgroup_files_legacy[9]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cftype cgroup_files[5]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct mutex resize_lock</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int nr_free_vmemmap_pages</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int demote_order</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int max_huge_pages_node[1024]</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int optimize_vmemmap_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_free_vmemmap_pages</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct cftype cgroup_files_dfl[7]</code> ➡️ <code>struct cftype cgroup_files_dfl[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct cftype cgroup_files_legacy[9]</code> ➡️ <code>struct cftype cgroup_files_legacy[10]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int optimize_vmemmap_pages</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct list_head hugepage_freelists[1024]</code> ➡️ <code>struct list_head hugepage_freelists[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int nr_huge_pages_node[1024]</code> ➡️ <code>unsigned int nr_huge_pages_node[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int free_huge_pages_node[1024]</code> ➡️ <code>unsigned int free_huge_pages_node[64]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int surplus_huge_pages_node[1024]</code> ➡️ <code>unsigned int surplus_huge_pages_node[64]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int next_nid_to_alloc</code>
</li>
<li>
<b>Field removed. </b>
<code>int next_nid_to_free</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int order</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mask</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int max_huge_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_huge_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int free_huge_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int resv_huge_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int surplus_huge_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_overcommit_huge_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head hugepage_activelist</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head hugepage_freelists[1024]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int nr_huge_pages_node[1024]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int free_huge_pages_node[1024]</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int surplus_huge_pages_node[1024]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct cftype cgroup_files[5]</code>
</li>
<li>
<b>Field removed. </b>
<code>char name[32]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct list_head hugepage_freelists[1024]</code> ➡️ <code>struct list_head hugepage_freelists[256]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int nr_huge_pages_node[1024]</code> ➡️ <code>unsigned int nr_huge_pages_node[256]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int free_huge_pages_node[1024]</code> ➡️ <code>unsigned int free_huge_pages_node[256]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int surplus_huge_pages_node[1024]</code> ➡️ <code>unsigned int surplus_huge_pages_node[256]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct list_head hugepage_freelists[1024]</code> ➡️ <code>struct list_head hugepage_freelists[1]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int nr_huge_pages_node[1024]</code> ➡️ <code>unsigned int nr_huge_pages_node[1]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int free_huge_pages_node[1024]</code> ➡️ <code>unsigned int free_huge_pages_node[1]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int surplus_huge_pages_node[1024]</code> ➡️ <code>unsigned int surplus_huge_pages_node[1]</code>
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
