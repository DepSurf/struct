# Struct: <code>load_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct load_info {
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct load_info {
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct load_info {
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug_info dyndbg;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct page **pages;
    unsigned int max_pages;
    unsigned int used_pages;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct page **pages;
    unsigned int max_pages;
    unsigned int used_pages;
    struct (anon) index;
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
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf32_Ehdr *hdr;
    long unsigned int len;
    Elf32_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
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
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct load_info {
    const char *name;
    struct module *mod;
    Elf64_Ehdr *hdr;
    long unsigned int len;
    Elf64_Shdr *sechdrs;
    char *secstrings;
    char *strtab;
    long unsigned int symoffs;
    long unsigned int stroffs;
    long unsigned int init_typeoffs;
    long unsigned int core_typeoffs;
    struct _ddebug *debug;
    unsigned int num_debug;
    bool sig_ok;
    long unsigned int mod_kallsyms_init_off;
    struct (anon) index;
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
<code>const char *name</code>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct module *mod</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int init_typeoffs</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int core_typeoffs</code>
</li>
</ul>
</details>
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct _ddebug_info dyndbg</code>
</li>
<li>
<b>Field removed. </b>
<code>struct _ddebug *debug</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int num_debug</code>
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
<code>struct page **pages</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int max_pages</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int used_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>struct _ddebug_info dyndbg</code>
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
<b>Field type changed. </b>
<code>Elf64_Ehdr *hdr</code> ➡️ <code>Elf32_Ehdr *hdr</code>
</li>
<li>
<b>Field type changed. </b>
<code>Elf64_Shdr *sechdrs</code> ➡️ <code>Elf32_Shdr *sechdrs</code>
</li>
</ul>
</details>
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
