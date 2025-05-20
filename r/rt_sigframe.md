# Struct: <code>rt_sigframe</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
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
struct rt_sigframe {
    struct siginfo info;
    struct ucontext uc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rt_sigframe {
    struct siginfo info;
    struct sigframe sig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rt_sigframe {
    compat_siginfo_t info;
    struct ucontext32 uc;
    struct ucontext32 uc_transact;
    int abigap[56];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rt_sigframe {
    struct siginfo info;
    struct ucontext uc;
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
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rt_sigframe {
    char *pretcode;
    struct ucontext uc;
    struct siginfo info;
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
<b>Field removed. </b>
<code>char *pretcode</code>
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
<code>struct sigframe sig</code>
</li>
<li>
<b>Field removed. </b>
<code>char *pretcode</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ucontext uc</code>
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
<code>struct ucontext32 uc_transact</code>
</li>
<li>
<b>Field added. </b>
<code>int abigap[56]</code>
</li>
<li>
<b>Field removed. </b>
<code>char *pretcode</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ucontext uc</code> ➡️ <code>struct ucontext32 uc</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct siginfo info</code> ➡️ <code>compat_siginfo_t info</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>char *pretcode</code>
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
