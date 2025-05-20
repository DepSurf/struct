# Struct: <code>kimage_arch</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kimage_arch {
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kimage_arch {
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kimage_arch {
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
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
struct kimage_arch {
    void *dtb;
    long unsigned int dtb_mem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kimage_arch {
    u32 kernel_r2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kimage_arch {
    phys_addr_t ima_buffer_addr;
    size_t ima_buffer_size;
};
```
</details>
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
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kimage_arch {
    p4d_t *p4d;
    pud_t *pud;
    pmd_t *pmd;
    pte_t *pte;
    long unsigned int backup_src_start;
    long unsigned int backup_src_sz;
    long unsigned int backup_load_addr;
    void *elf_headers;
    long unsigned int elf_headers_sz;
    long unsigned int elf_load_addr;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>p4d_t *p4d</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>long unsigned int backup_src_start</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_src_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_load_addr</code>
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
<b>Field removed. </b>
<code>void *elf_headers</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_headers_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_load_addr</code>
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
<b>Field added. </b>
<code>void *dtb</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int dtb_mem</code>
</li>
<li>
<b>Field removed. </b>
<code>p4d_t *p4d</code>
</li>
<li>
<b>Field removed. </b>
<code>pud_t *pud</code>
</li>
<li>
<b>Field removed. </b>
<code>pmd_t *pmd</code>
</li>
<li>
<b>Field removed. </b>
<code>pte_t *pte</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_src_start</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_src_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_load_addr</code>
</li>
<li>
<b>Field removed. </b>
<code>void *elf_headers</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_headers_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_load_addr</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 kernel_r2</code>
</li>
<li>
<b>Field removed. </b>
<code>p4d_t *p4d</code>
</li>
<li>
<b>Field removed. </b>
<code>pud_t *pud</code>
</li>
<li>
<b>Field removed. </b>
<code>pmd_t *pmd</code>
</li>
<li>
<b>Field removed. </b>
<code>pte_t *pte</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_src_start</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_src_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_load_addr</code>
</li>
<li>
<b>Field removed. </b>
<code>void *elf_headers</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_headers_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_load_addr</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>phys_addr_t ima_buffer_addr</code>
</li>
<li>
<b>Field added. </b>
<code>size_t ima_buffer_size</code>
</li>
<li>
<b>Field removed. </b>
<code>p4d_t *p4d</code>
</li>
<li>
<b>Field removed. </b>
<code>pud_t *pud</code>
</li>
<li>
<b>Field removed. </b>
<code>pmd_t *pmd</code>
</li>
<li>
<b>Field removed. </b>
<code>pte_t *pte</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_src_start</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_src_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int backup_load_addr</code>
</li>
<li>
<b>Field removed. </b>
<code>void *elf_headers</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_headers_sz</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int elf_load_addr</code>
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
