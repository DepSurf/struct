# Struct: <code>pv_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    int paravirt_enabled;
    unsigned int features;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pv_info {
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pv_info {
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pv_info {
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pv_info {
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pv_info {
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pv_info {
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pv_info {
    u16 extra_user_64bit_cs;
    const char *name;
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
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct pv_info {
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pv_info {
    unsigned int kernel_rpl;
    int shared_kernel_pmd;
    u16 extra_user_64bit_cs;
    const char *name;
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
<code>int paravirt_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int features</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int kernel_rpl</code>
</li>
<li>
<b>Field removed. </b>
<code>int shared_kernel_pmd</code>
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
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int kernel_rpl</code>
</li>
<li>
<b>Field removed. </b>
<code>int shared_kernel_pmd</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 extra_user_64bit_cs</code>
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
