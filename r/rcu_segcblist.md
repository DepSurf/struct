# Struct: <code>rcu_segcblist</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int seglen[4];
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int seglen[4];
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int seglen[4];
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int seglen[4];
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int seglen[4];
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    atomic_long_t len;
    long int seglen[4];
    u8 flags;
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
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
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
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    atomic_long_t len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rcu_segcblist {
    struct callback_head *head;
    struct callback_head ** tails[4];
    long unsigned int gp_seq[4];
    long int len;
    long int len_lazy;
    u8 enabled;
    u8 offloaded;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 enabled</code>
</li>
<li>
<b>Field added. </b>
<code>u8 offloaded</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long int len_lazy</code>
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
<b>Field added. </b>
<code>long int seglen[4]</code>
</li>
<li>
<b>Field added. </b>
<code>u8 flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 offloaded</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int len</code> ➡️ <code>atomic_long_t len</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int len</code> ➡️ <code>atomic_long_t len</code>
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
