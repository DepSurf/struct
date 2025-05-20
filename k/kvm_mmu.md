# Struct: <code>kvm_mmu</code>

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
In <code>5.8</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kvm_mmu {
    long unsigned int (*get_guest_pgd)(struct kvm_vcpu *);
    u64 (*get_pdptr)(struct kvm_vcpu *, int);
    int (*page_fault)(struct kvm_vcpu *, gpa_t, u32, bool);
    void (*inject_page_fault)(struct kvm_vcpu *, struct x86_exception *);
    gpa_t (*gva_to_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *);
    gpa_t (*translate_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *);
    int (*sync_page)(struct kvm_vcpu *, struct kvm_mmu_page *);
    void (*invlpg)(struct kvm_vcpu *, gva_t, hpa_t);
    void (*update_pte)(struct kvm_vcpu *, struct kvm_mmu_page *, u64 *, const void *);
    hpa_t root_hpa;
    gpa_t root_pgd;
    union kvm_mmu_role mmu_role;
    u8 root_level;
    u8 shadow_root_level;
    u8 ept_ad;
    bool direct_map;
    struct kvm_mmu_root_info prev_roots[3];
    u8 permissions[16];
    u32 pkru_mask;
    u64 *pae_root;
    u64 *lm_root;
    struct rsvd_bits_validate shadow_zero_check;
    struct rsvd_bits_validate guest_rsvd_check;
    u8 last_nonleaf_level;
    bool nx;
    u64 pdptrs[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_mmu {
    long unsigned int (*get_guest_pgd)(struct kvm_vcpu *);
    u64 (*get_pdptr)(struct kvm_vcpu *, int);
    int (*page_fault)(struct kvm_vcpu *, gpa_t, u32, bool);
    void (*inject_page_fault)(struct kvm_vcpu *, struct x86_exception *);
    gpa_t (*gva_to_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *);
    gpa_t (*translate_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *);
    int (*sync_page)(struct kvm_vcpu *, struct kvm_mmu_page *);
    void (*invlpg)(struct kvm_vcpu *, gva_t, hpa_t);
    hpa_t root_hpa;
    gpa_t root_pgd;
    union kvm_mmu_role mmu_role;
    u8 root_level;
    u8 shadow_root_level;
    u8 ept_ad;
    bool direct_map;
    struct kvm_mmu_root_info prev_roots[3];
    u8 permissions[16];
    u32 pkru_mask;
    u64 *pae_root;
    u64 *pml4_root;
    struct rsvd_bits_validate shadow_zero_check;
    struct rsvd_bits_validate guest_rsvd_check;
    u8 last_nonleaf_level;
    bool nx;
    u64 pdptrs[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_mmu {
    long unsigned int (*get_guest_pgd)(struct kvm_vcpu *);
    u64 (*get_pdptr)(struct kvm_vcpu *, int);
    int (*page_fault)(struct kvm_vcpu *, gpa_t, u32, bool);
    void (*inject_page_fault)(struct kvm_vcpu *, struct x86_exception *);
    gpa_t (*gva_to_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *);
    gpa_t (*translate_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *);
    int (*sync_page)(struct kvm_vcpu *, struct kvm_mmu_page *);
    void (*invlpg)(struct kvm_vcpu *, gva_t, hpa_t);
    hpa_t root_hpa;
    gpa_t root_pgd;
    union kvm_mmu_role mmu_role;
    u8 root_level;
    u8 shadow_root_level;
    u8 ept_ad;
    bool direct_map;
    struct kvm_mmu_root_info prev_roots[3];
    u8 permissions[16];
    u32 pkru_mask;
    u64 *pae_root;
    u64 *pml4_root;
    u64 *pml5_root;
    struct rsvd_bits_validate shadow_zero_check;
    struct rsvd_bits_validate guest_rsvd_check;
    u64 pdptrs[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_mmu {
    long unsigned int (*get_guest_pgd)(struct kvm_vcpu *);
    u64 (*get_pdptr)(struct kvm_vcpu *, int);
    int (*page_fault)(struct kvm_vcpu *, struct kvm_page_fault *);
    void (*inject_page_fault)(struct kvm_vcpu *, struct x86_exception *);
    gpa_t (*gva_to_gpa)(struct kvm_vcpu *, struct kvm_mmu *, gpa_t, u64, struct x86_exception *);
    int (*sync_page)(struct kvm_vcpu *, struct kvm_mmu_page *);
    void (*invlpg)(struct kvm_vcpu *, gva_t, hpa_t);
    struct kvm_mmu_root_info root;
    union kvm_cpu_role cpu_role;
    union kvm_mmu_page_role root_role;
    u32 pkru_mask;
    struct kvm_mmu_root_info prev_roots[3];
    u8 permissions[16];
    u64 *pae_root;
    u64 *pml4_root;
    u64 *pml5_root;
    struct rsvd_bits_validate shadow_zero_check;
    struct rsvd_bits_validate guest_rsvd_check;
    u64 pdptrs[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_mmu {
    long unsigned int (*get_guest_pgd)(struct kvm_vcpu *);
    u64 (*get_pdptr)(struct kvm_vcpu *, int);
    int (*page_fault)(struct kvm_vcpu *, struct kvm_page_fault *);
    void (*inject_page_fault)(struct kvm_vcpu *, struct x86_exception *);
    gpa_t (*gva_to_gpa)(struct kvm_vcpu *, struct kvm_mmu *, gpa_t, u64, struct x86_exception *);
    int (*sync_page)(struct kvm_vcpu *, struct kvm_mmu_page *);
    void (*invlpg)(struct kvm_vcpu *, gva_t, hpa_t);
    struct kvm_mmu_root_info root;
    union kvm_cpu_role cpu_role;
    union kvm_mmu_page_role root_role;
    u32 pkru_mask;
    struct kvm_mmu_root_info prev_roots[3];
    u8 permissions[16];
    u64 *pae_root;
    u64 *pml4_root;
    u64 *pml5_root;
    struct rsvd_bits_validate shadow_zero_check;
    struct rsvd_bits_validate guest_rsvd_check;
    u64 pdptrs[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_mmu {
    long unsigned int (*get_guest_pgd)(struct kvm_vcpu *);
    u64 (*get_pdptr)(struct kvm_vcpu *, int);
    int (*page_fault)(struct kvm_vcpu *, struct kvm_page_fault *);
    void (*inject_page_fault)(struct kvm_vcpu *, struct x86_exception *);
    gpa_t (*gva_to_gpa)(struct kvm_vcpu *, struct kvm_mmu *, gpa_t, u64, struct x86_exception *);
    int (*sync_spte)(struct kvm_vcpu *, struct kvm_mmu_page *, int);
    struct kvm_mmu_root_info root;
    union kvm_cpu_role cpu_role;
    union kvm_mmu_page_role root_role;
    u32 pkru_mask;
    struct kvm_mmu_root_info prev_roots[3];
    u8 permissions[16];
    u64 *pae_root;
    u64 *pml4_root;
    u64 *pml5_root;
    struct rsvd_bits_validate shadow_zero_check;
    struct rsvd_bits_validate guest_rsvd_check;
    u64 pdptrs[4];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_mmu {
    long unsigned int (*get_guest_pgd)(struct kvm_vcpu *);
    u64 (*get_pdptr)(struct kvm_vcpu *, int);
    int (*page_fault)(struct kvm_vcpu *, struct kvm_page_fault *);
    void (*inject_page_fault)(struct kvm_vcpu *, struct x86_exception *);
    gpa_t (*gva_to_gpa)(struct kvm_vcpu *, struct kvm_mmu *, gpa_t, u64, struct x86_exception *);
    int (*sync_spte)(struct kvm_vcpu *, struct kvm_mmu_page *, int);
    struct kvm_mmu_root_info root;
    union kvm_cpu_role cpu_role;
    union kvm_mmu_page_role root_role;
    u32 pkru_mask;
    struct kvm_mmu_root_info prev_roots[3];
    u8 permissions[16];
    u64 *pae_root;
    u64 *pml4_root;
    u64 *pml5_root;
    struct rsvd_bits_validate shadow_zero_check;
    struct rsvd_bits_validate guest_rsvd_check;
    u64 pdptrs[4];
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 *pml4_root</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*update_pte)(struct kvm_vcpu *, struct kvm_mmu_page *, u64 *, const void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 *lm_root</code>
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
<code>u64 *pml5_root</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 last_nonleaf_level</code>
</li>
<li>
<b>Field removed. </b>
<code>bool nx</code>
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
<code>struct kvm_mmu_root_info root</code>
</li>
<li>
<b>Field added. </b>
<code>union kvm_cpu_role cpu_role</code>
</li>
<li>
<b>Field added. </b>
<code>union kvm_mmu_page_role root_role</code>
</li>
<li>
<b>Field removed. </b>
<code>gpa_t (*translate_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *)</code>
</li>
<li>
<b>Field removed. </b>
<code>hpa_t root_hpa</code>
</li>
<li>
<b>Field removed. </b>
<code>gpa_t root_pgd</code>
</li>
<li>
<b>Field removed. </b>
<code>union kvm_mmu_role mmu_role</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 root_level</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 shadow_root_level</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 ept_ad</code>
</li>
<li>
<b>Field removed. </b>
<code>bool direct_map</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*page_fault)(struct kvm_vcpu *, gpa_t, u32, bool)</code> ➡️ <code>int (*page_fault)(struct kvm_vcpu *, struct kvm_page_fault *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>gpa_t (*gva_to_gpa)(struct kvm_vcpu *, gpa_t, u32, struct x86_exception *)</code> ➡️ <code>gpa_t (*gva_to_gpa)(struct kvm_vcpu *, struct kvm_mmu *, gpa_t, u64, struct x86_exception *)</code>
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
<code>int (*sync_spte)(struct kvm_vcpu *, struct kvm_mmu_page *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*sync_page)(struct kvm_vcpu *, struct kvm_mmu_page *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*invlpg)(struct kvm_vcpu *, gva_t, hpa_t)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
