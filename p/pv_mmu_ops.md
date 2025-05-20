# Struct: <code>pv_mmu_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pv_mmu_ops {
    long unsigned int (*read_cr2)();
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    void (*exit_mmap)(struct mm_struct *);
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_single)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    void (*set_pmd_at)(struct mm_struct *, long unsigned int, pmd_t *, pmd_t);
    void (*pte_update)(struct mm_struct *, long unsigned int, pte_t *);
    void (*pte_update_defer)(struct mm_struct *, long unsigned int, pte_t *);
    void (*pmd_update)(struct mm_struct *, long unsigned int, pmd_t *);
    void (*pmd_update_defer)(struct mm_struct *, long unsigned int, pmd_t *);
    pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pv_mmu_ops {
    long unsigned int (*read_cr2)();
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    void (*exit_mmap)(struct mm_struct *);
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_single)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    void (*set_pmd_at)(struct mm_struct *, long unsigned int, pmd_t *, pmd_t);
    void (*pte_update)(struct mm_struct *, long unsigned int, pte_t *);
    pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pv_mmu_ops {
    long unsigned int (*read_cr2)();
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    void (*exit_mmap)(struct mm_struct *);
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_single)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, struct mm_struct *, long unsigned int, long unsigned int);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    void (*set_pmd_at)(struct mm_struct *, long unsigned int, pmd_t *, pmd_t);
    void (*pte_update)(struct mm_struct *, long unsigned int, pte_t *);
    pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pv_mmu_ops {
    long unsigned int (*read_cr2)();
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    void (*exit_mmap)(struct mm_struct *);
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_single)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    void (*set_pmd_at)(struct mm_struct *, long unsigned int, pmd_t *, pmd_t);
    void (*set_pud_at)(struct mm_struct *, long unsigned int, pud_t *, pud_t);
    void (*pte_update)(struct mm_struct *, long unsigned int, pte_t *);
    pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pv_mmu_ops {
    long unsigned int (*read_cr2)();
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    void (*exit_mmap)(struct mm_struct *);
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pv_mmu_ops {
    long unsigned int (*read_cr2)();
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    void (*exit_mmap)(struct mm_struct *);
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    long unsigned int (*read_cr2)();
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_multi)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_multi)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_multi)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    void (*notify_page_enc_status_changed)(long unsigned int, int, bool);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_multi)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    void (*notify_page_enc_status_changed)(long unsigned int, int, bool);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_multi)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    void (*notify_page_enc_status_changed)(long unsigned int, int, bool);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*enter_mmap)(struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_multi)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    void (*notify_page_enc_status_changed)(long unsigned int, int, bool);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*enter_mmap)(struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct paravirt_callee_save p4d_val;
    struct paravirt_callee_save make_p4d;
    void (*set_pgd)(pgd_t *, pgd_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pv_mmu_ops {
    void (*flush_tlb_user)();
    void (*flush_tlb_kernel)();
    void (*flush_tlb_one_user)(long unsigned int);
    void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *);
    void (*tlb_remove_table)(struct mmu_gather *, void *);
    void (*exit_mmap)(struct mm_struct *);
    struct paravirt_callee_save read_cr2;
    void (*write_cr2)(long unsigned int);
    long unsigned int (*read_cr3)();
    void (*write_cr3)(long unsigned int);
    void (*activate_mm)(struct mm_struct *, struct mm_struct *);
    void (*dup_mmap)(struct mm_struct *, struct mm_struct *);
    int (*pgd_alloc)(struct mm_struct *);
    void (*pgd_free)(struct mm_struct *, pgd_t *);
    void (*alloc_pte)(struct mm_struct *, long unsigned int);
    void (*alloc_pmd)(struct mm_struct *, long unsigned int);
    void (*alloc_pud)(struct mm_struct *, long unsigned int);
    void (*alloc_p4d)(struct mm_struct *, long unsigned int);
    void (*release_pte)(long unsigned int);
    void (*release_pmd)(long unsigned int);
    void (*release_pud)(long unsigned int);
    void (*release_p4d)(long unsigned int);
    void (*set_pte)(pte_t *, pte_t);
    void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t);
    void (*set_pmd)(pmd_t *, pmd_t);
    pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *);
    void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t);
    struct paravirt_callee_save pte_val;
    struct paravirt_callee_save make_pte;
    struct paravirt_callee_save pgd_val;
    struct paravirt_callee_save make_pgd;
    void (*set_pud)(pud_t *, pud_t);
    struct paravirt_callee_save pmd_val;
    struct paravirt_callee_save make_pmd;
    struct paravirt_callee_save pud_val;
    struct paravirt_callee_save make_pud;
    void (*set_p4d)(p4d_t *, p4d_t);
    struct pv_lazy_ops lazy_mode;
    void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t);
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
<b>Field removed. </b>
<code>void (*pte_update_defer)(struct mm_struct *, long unsigned int, pte_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*pmd_update)(struct mm_struct *, long unsigned int, pmd_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*pmd_update_defer)(struct mm_struct *, long unsigned int, pmd_t *)</code>
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
<code>void (*alloc_p4d)(struct mm_struct *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*release_p4d)(long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*set_pud_at)(struct mm_struct *, long unsigned int, pud_t *, pud_t)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*set_p4d)(p4d_t *, p4d_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_pgd)(pgd_t *, pgd_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*flush_tlb_others)(const struct cpumask *, struct mm_struct *, long unsigned int, long unsigned int)</code> ➡️ <code>void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *)</code>
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
<code>void (*flush_tlb_one_user)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*flush_tlb_single)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_pmd_at)(struct mm_struct *, long unsigned int, pmd_t *, pmd_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_pud_at)(struct mm_struct *, long unsigned int, pud_t *, pud_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*pte_update)(struct mm_struct *, long unsigned int, pte_t *)</code>
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
<code>void (*tlb_remove_table)(struct mmu_gather *, void *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int (*read_cr2)()</code> ➡️ <code>struct paravirt_callee_save read_cr2</code>
</li>
<li>
<b>Field type changed. </b>
<code>pte_t (*ptep_modify_prot_start)(struct mm_struct *, long unsigned int, pte_t *)</code> ➡️ <code>pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*ptep_modify_prot_commit)(struct mm_struct *, long unsigned int, pte_t *, pte_t)</code> ➡️ <code>void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t)</code>
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
<code>struct paravirt_callee_save p4d_val</code>
</li>
<li>
<b>Field added. </b>
<code>struct paravirt_callee_save make_p4d</code>
</li>
<li>
<b>Field added. </b>
<code>void (*set_pgd)(pgd_t *, pgd_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*flush_tlb_multi)(const struct cpumask *, const struct flush_tlb_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*flush_tlb_others)(const struct cpumask *, const struct flush_tlb_info *)</code>
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
<code>void (*notify_page_enc_status_changed)(long unsigned int, int, bool)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*enter_mmap)(struct mm_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*activate_mm)(struct mm_struct *, struct mm_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*dup_mmap)(struct mm_struct *, struct mm_struct *)</code>
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
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save read_cr2</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_cr2)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int (*read_cr3)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*write_cr3)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*activate_mm)(struct mm_struct *, struct mm_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*dup_mmap)(struct mm_struct *, struct mm_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*pgd_alloc)(struct mm_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*pgd_free)(struct mm_struct *, pgd_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*alloc_pte)(struct mm_struct *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*alloc_pmd)(struct mm_struct *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*alloc_pud)(struct mm_struct *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*alloc_p4d)(struct mm_struct *, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*release_pte)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*release_pmd)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*release_pud)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*release_p4d)(long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_pte)(pte_t *, pte_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_pte_at)(struct mm_struct *, long unsigned int, pte_t *, pte_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_pmd)(pmd_t *, pmd_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>pte_t (*ptep_modify_prot_start)(struct vm_area_struct *, long unsigned int, pte_t *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*ptep_modify_prot_commit)(struct vm_area_struct *, long unsigned int, pte_t *, pte_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save pte_val</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save make_pte</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save pgd_val</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save make_pgd</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_pud)(pud_t *, pud_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save pmd_val</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save make_pmd</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save pud_val</code>
</li>
<li>
<b>Field removed. </b>
<code>struct paravirt_callee_save make_pud</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_p4d)(p4d_t *, p4d_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_lazy_ops lazy_mode</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_fixmap)(unsigned int, phys_addr_t, pgprot_t)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
