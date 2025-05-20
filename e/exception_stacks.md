# Struct: <code>exception_stacks</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB2_stack_guard[0];
    char DB2_stack[0];
    char DB1_stack_guard[0];
    char DB1_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB2_stack_guard[0];
    char DB2_stack[0];
    char DB1_stack_guard[0];
    char DB1_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char VC_stack_guard[0];
    char VC_stack[0];
    char VC2_stack_guard[0];
    char VC2_stack[0];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char VC_stack_guard[0];
    char VC_stack[0];
    char VC2_stack_guard[0];
    char VC2_stack[0];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[8192];
    char NMI_stack_guard[0];
    char NMI_stack[8192];
    char DB_stack_guard[0];
    char DB_stack[8192];
    char MCE_stack_guard[0];
    char MCE_stack[8192];
    char VC_stack_guard[0];
    char VC_stack[8192];
    char VC2_stack_guard[0];
    char VC2_stack[8192];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[8192];
    char NMI_stack_guard[0];
    char NMI_stack[8192];
    char DB_stack_guard[0];
    char DB_stack[8192];
    char MCE_stack_guard[0];
    char MCE_stack[8192];
    char VC_stack_guard[0];
    char VC_stack[8192];
    char VC2_stack_guard[0];
    char VC2_stack[8192];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[8192];
    char NMI_stack_guard[0];
    char NMI_stack[8192];
    char DB_stack_guard[0];
    char DB_stack[8192];
    char MCE_stack_guard[0];
    char MCE_stack[8192];
    char VC_stack_guard[0];
    char VC_stack[8192];
    char VC2_stack_guard[0];
    char VC2_stack[8192];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[8192];
    char NMI_stack_guard[0];
    char NMI_stack[8192];
    char DB_stack_guard[0];
    char DB_stack[8192];
    char MCE_stack_guard[0];
    char MCE_stack[8192];
    char VC_stack_guard[0];
    char VC_stack[8192];
    char VC2_stack_guard[0];
    char VC2_stack[8192];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[8192];
    char NMI_stack_guard[0];
    char NMI_stack[8192];
    char DB_stack_guard[0];
    char DB_stack[8192];
    char MCE_stack_guard[0];
    char MCE_stack[8192];
    char VC_stack_guard[0];
    char VC_stack[8192];
    char VC2_stack_guard[0];
    char VC2_stack[8192];
    char IST_top_guard[0];
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
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB2_stack_guard[0];
    char DB2_stack[0];
    char DB1_stack_guard[0];
    char DB1_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB2_stack_guard[0];
    char DB2_stack[0];
    char DB1_stack_guard[0];
    char DB1_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB2_stack_guard[0];
    char DB2_stack[0];
    char DB1_stack_guard[0];
    char DB1_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char IST_top_guard[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct exception_stacks {
    char DF_stack_guard[0];
    char DF_stack[4096];
    char NMI_stack_guard[0];
    char NMI_stack[4096];
    char DB2_stack_guard[0];
    char DB2_stack[0];
    char DB1_stack_guard[0];
    char DB1_stack[4096];
    char DB_stack_guard[0];
    char DB_stack[4096];
    char MCE_stack_guard[0];
    char MCE_stack[4096];
    char IST_top_guard[0];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>char DB2_stack_guard[0]</code>
</li>
<li>
<b>Field removed. </b>
<code>char DB2_stack[0]</code>
</li>
<li>
<b>Field removed. </b>
<code>char DB1_stack_guard[0]</code>
</li>
<li>
<b>Field removed. </b>
<code>char DB1_stack[4096]</code>
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
<code>char VC_stack_guard[0]</code>
</li>
<li>
<b>Field added. </b>
<code>char VC_stack[0]</code>
</li>
<li>
<b>Field added. </b>
<code>char VC2_stack_guard[0]</code>
</li>
<li>
<b>Field added. </b>
<code>char VC2_stack[0]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char DF_stack[4096]</code> ➡️ <code>char DF_stack[8192]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char NMI_stack[4096]</code> ➡️ <code>char NMI_stack[8192]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char DB_stack[4096]</code> ➡️ <code>char DB_stack[8192]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char MCE_stack[4096]</code> ➡️ <code>char MCE_stack[8192]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char VC_stack[0]</code> ➡️ <code>char VC_stack[8192]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char VC2_stack[0]</code> ➡️ <code>char VC2_stack[8192]</code>
</li>
</ul>
</details>
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
