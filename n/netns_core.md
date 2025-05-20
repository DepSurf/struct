# Struct: <code>netns_core</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    struct prot_inuse *inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    struct prot_inuse *inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    struct prot_inuse *inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    struct prot_inuse *inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    struct prot_inuse *inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    u8 sysctl_txrehash;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    u8 sysctl_txrehash;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    u8 sysctl_txrehash;
    struct prot_inuse *prot_inuse;
    struct cpumask *rps_default_mask;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int sysctl_optmem_max;
    u8 sysctl_txrehash;
    struct prot_inuse *prot_inuse;
    struct cpumask *rps_default_mask;
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
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
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
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct netns_core {
    struct ctl_table_header *sysctl_hdr;
    int sysctl_somaxconn;
    int *sock_inuse;
    struct prot_inuse *prot_inuse;
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int *sock_inuse</code>
</li>
<li>
<b>Field added. </b>
<code>struct prot_inuse *prot_inuse</code>
</li>
<li>
<b>Field removed. </b>
<code>struct prot_inuse *inuse</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 sysctl_txrehash</code>
</li>
<li>
<b>Field removed. </b>
<code>int *sock_inuse</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cpumask *rps_default_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int sysctl_optmem_max</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
