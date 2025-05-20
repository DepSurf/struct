# Struct: <code>uncharge_gather</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_pages;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_pages;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_memory;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_memory;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_memory;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    int nid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_memory;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    int nid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_memory;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    int nid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int nr_memory;
    long unsigned int pgpgout;
    long unsigned int nr_kmem;
    int nid;
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
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
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
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uncharge_gather {
    struct mem_cgroup *memcg;
    long unsigned int pgpgout;
    long unsigned int nr_anon;
    long unsigned int nr_file;
    long unsigned int nr_kmem;
    long unsigned int nr_huge;
    long unsigned int nr_shmem;
    struct page *dummy_page;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int nr_pages</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_anon</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_file</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_huge</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_shmem</code>
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
<code>long unsigned int nr_memory</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int nr_pages</code>
</li>
</ul>
</details>
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
<code>int nid</code>
</li>
<li>
<b>Field removed. </b>
<code>struct page *dummy_page</code>
</li>
</ul>
</details>
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
