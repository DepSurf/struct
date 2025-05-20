# Struct: <code>user</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct user {
    struct user_regs_struct regs;
    int u_fpvalid;
    int pad0;
    struct user_i387_struct i387;
    long unsigned int u_tsize;
    long unsigned int u_dsize;
    long unsigned int u_ssize;
    long unsigned int start_code;
    long unsigned int start_stack;
    long int signal;
    int reserved;
    int pad1;
    long unsigned int u_ar0;
    struct user_i387_struct *u_fpstate;
    long unsigned int magic;
    char u_comm[32];
    long unsigned int u_debugreg[8];
    long unsigned int error_code;
    long unsigned int fault_address;
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
