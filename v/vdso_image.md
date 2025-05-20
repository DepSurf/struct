# Struct: <code>vdso_image</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    struct vm_special_mapping text_mapping;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_hpet_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_hpet_page;
    long int sym_pvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_hpet_page;
    long int sym_pvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_hpet_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_hpet_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_hpet_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_hpet_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long unsigned int extable_base;
    long unsigned int extable_len;
    const void *extable;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
    long int sym_vdso32_sigreturn_landing_pad;
    long int sym_vdso32_rt_sigreturn_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long unsigned int extable_base;
    long unsigned int extable_len;
    const void *extable;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
    long int sym_vdso32_sigreturn_landing_pad;
    long int sym_vdso32_rt_sigreturn_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long unsigned int extable_base;
    long unsigned int extable_len;
    const void *extable;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
    long int sym_vdso32_sigreturn_landing_pad;
    long int sym_vdso32_rt_sigreturn_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long unsigned int extable_base;
    long unsigned int extable_len;
    const void *extable;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
    long int sym_vdso32_sigreturn_landing_pad;
    long int sym_vdso32_rt_sigreturn_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long unsigned int extable_base;
    long unsigned int extable_len;
    const void *extable;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
    long int sym_vdso32_sigreturn_landing_pad;
    long int sym_vdso32_rt_sigreturn_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long unsigned int extable_base;
    long unsigned int extable_len;
    const void *extable;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
    long int sym_vdso32_sigreturn_landing_pad;
    long int sym_vdso32_rt_sigreturn_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long unsigned int extable_base;
    long unsigned int extable_len;
    const void *extable;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_timens_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
    long int sym_vdso32_sigreturn_landing_pad;
    long int sym_vdso32_rt_sigreturn_landing_pad;
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
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vdso_image {
    void *data;
    long unsigned int size;
    long unsigned int alt;
    long unsigned int alt_len;
    long int sym_vvar_start;
    long int sym_vvar_page;
    long int sym_pvclock_page;
    long int sym_hvclock_page;
    long int sym_VDSO32_NOTE_MASK;
    long int sym___kernel_sigreturn;
    long int sym___kernel_rt_sigreturn;
    long int sym___kernel_vsyscall;
    long int sym_int80_landing_pad;
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
<b>Field added. </b>
<code>long int sym_pvclock_page</code>
</li>
<li>
<b>Field removed. </b>
<code>struct vm_special_mapping text_mapping</code>
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
<code>long int sym_hvclock_page</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long int sym_hpet_page</code>
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
<code>long int sym_timens_page</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int extable_base</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int extable_len</code>
</li>
<li>
<b>Field added. </b>
<code>const void *extable</code>
</li>
<li>
<b>Field added. </b>
<code>long int sym_vdso32_sigreturn_landing_pad</code>
</li>
<li>
<b>Field added. </b>
<code>long int sym_vdso32_rt_sigreturn_landing_pad</code>
</li>
</ul>
</details>
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
No changes between <code>6.2</code> and <code>6.5</code> ✅
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
