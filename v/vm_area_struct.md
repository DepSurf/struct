# Struct: <code>vm_area_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct anon_vma_name *anon_name;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    struct anon_vma_name *anon_name;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct callback_head vm_rcu;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    const vm_flags_t vm_flags;
    vm_flags_t __vm_flags;
    int vm_lock_seq;
    struct vma_lock *vm_lock;
    bool detached;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    void *vm_private_data;
    struct anon_vma_name *anon_name;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vma_numab_state *numab_state;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct callback_head vm_rcu;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    const vm_flags_t vm_flags;
    vm_flags_t __vm_flags;
    int vm_lock_seq;
    struct vma_lock *vm_lock;
    bool detached;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    void *vm_private_data;
    struct anon_vma_name *anon_name;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vma_numab_state *numab_state;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
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
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
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
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vm_area_struct {
    long unsigned int vm_start;
    long unsigned int vm_end;
    struct vm_area_struct *vm_next;
    struct vm_area_struct *vm_prev;
    struct rb_node vm_rb;
    long unsigned int rb_subtree_gap;
    struct mm_struct *vm_mm;
    pgprot_t vm_page_prot;
    long unsigned int vm_flags;
    struct (anon) shared;
    struct list_head anon_vma_chain;
    struct anon_vma *anon_vma;
    const struct vm_operations_struct *vm_ops;
    long unsigned int vm_pgoff;
    struct file *vm_file;
    struct file *vm_prfile;
    void *vm_private_data;
    atomic_long_t swap_readahead_info;
    struct mempolicy *vm_policy;
    struct vm_userfaultfd_ctx vm_userfaultfd_ctx;
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
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>atomic_long_t swap_readahead_info</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct file *vm_prfile</code>
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
<code>struct file *vm_prfile</code>
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
<code>struct anon_vma_name *anon_name</code>
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
<code>struct vm_area_struct *vm_next</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vm_area_struct *vm_prev</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rb_node vm_rb</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int rb_subtree_gap</code>
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
<code>struct callback_head vm_rcu</code>
</li>
<li>
<b>Field added. </b>
<code>vm_flags_t __vm_flags</code>
</li>
<li>
<b>Field added. </b>
<code>int vm_lock_seq</code>
</li>
<li>
<b>Field added. </b>
<code>struct vma_lock *vm_lock</code>
</li>
<li>
<b>Field added. </b>
<code>bool detached</code>
</li>
<li>
<b>Field added. </b>
<code>struct vma_numab_state *numab_state</code>
</li>
<li>
<b>Field removed. </b>
<code>struct file *vm_prfile</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int vm_flags</code> ➡️ <code>const vm_flags_t vm_flags</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct mempolicy *vm_policy</code>
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
<code>struct mempolicy *vm_policy</code>
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
