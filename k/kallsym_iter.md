# Struct: <code>kallsym_iter</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    loff_t pos_bpf_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    loff_t pos_bpf_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    loff_t pos_bpf_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    loff_t pos_bpf_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    loff_t pos_bpf_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[512];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    loff_t pos_bpf_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[512];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    loff_t pos_bpf_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[512];
    char module_name[56];
    int exported;
    int show_value;
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
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[60];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
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
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kallsym_iter {
    loff_t pos;
    loff_t pos_arch_end;
    loff_t pos_mod_end;
    loff_t pos_ftrace_mod_end;
    long unsigned int value;
    unsigned int nameoff;
    char type;
    char name[128];
    char module_name[56];
    int exported;
    int show_value;
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
<code>loff_t pos_mod_end</code>
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
<code>loff_t pos_ftrace_mod_end</code>
</li>
<li>
<b>Field added. </b>
<code>int show_value</code>
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
<code>loff_t pos_arch_end</code>
</li>
</ul>
</details>
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
<code>loff_t pos_bpf_end</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char name[128]</code> ➡️ <code>char name[512]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>loff_t pos_arch_end</code>
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
<code>char module_name[56]</code> ➡️ <code>char module_name[60]</code>
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
