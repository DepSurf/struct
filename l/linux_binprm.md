# Struct: <code>linux_binprm</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct linux_binprm {
    char buf[128];
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    unsigned int cred_prepared;
    unsigned int cap_effective;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct linux_binprm {
    char buf[128];
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    unsigned int cred_prepared;
    unsigned int cap_effective;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct linux_binprm {
    char buf[128];
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    unsigned int cred_prepared;
    unsigned int cap_effective;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct linux_binprm {
    char buf[128];
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    unsigned int cred_prepared;
    unsigned int cap_effective;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct linux_binprm {
    char buf[128];
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct linux_binprm {
    char buf[128];
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct linux_binprm {
    char buf[128];
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    const char *fdpath;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    const char *fdpath;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    const char *fdpath;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    const char *fdpath;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    const char *fdpath;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    const char *fdpath;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int have_execfd;
    unsigned int execfd_creds;
    unsigned int secureexec;
    unsigned int point_of_no_return;
    struct file *executable;
    struct file *interpreter;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    const char *fdpath;
    unsigned int interp_flags;
    int execfd;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
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
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
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
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct linux_binprm {
    struct vm_area_struct *vma;
    long unsigned int vma_pages;
    struct mm_struct *mm;
    long unsigned int p;
    long unsigned int argmin;
    unsigned int called_set_creds;
    unsigned int cap_elevated;
    unsigned int secureexec;
    unsigned int recursion_depth;
    struct file *file;
    struct cred *cred;
    int unsafe;
    unsigned int per_clear;
    int argc;
    int envc;
    const char *filename;
    const char *interp;
    unsigned int interp_flags;
    unsigned int interp_data;
    long unsigned int loader;
    long unsigned int exec;
    struct rlimit rlim_stack;
    char buf[256];
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
<code>unsigned int called_set_creds</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int cap_elevated</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int secureexec</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int cred_prepared</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int cap_effective</code>
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
<code>struct rlimit rlim_stack</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int argmin</code>
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
<code>char buf[128]</code> ➡️ <code>char buf[256]</code>
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
<code>unsigned int have_execfd</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int execfd_creds</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int point_of_no_return</code>
</li>
<li>
<b>Field added. </b>
<code>struct file *executable</code>
</li>
<li>
<b>Field added. </b>
<code>struct file *interpreter</code>
</li>
<li>
<b>Field added. </b>
<code>int execfd</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int called_set_creds</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int cap_elevated</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int recursion_depth</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int interp_data</code>
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
<code>const char *fdpath</code>
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
