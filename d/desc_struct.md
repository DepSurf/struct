# Struct: <code>desc_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct desc_struct {
    unsigned int a;
    unsigned int b;
    u16 limit0;
    u16 base0;
    unsigned int base1;
    unsigned int type;
    unsigned int s;
    unsigned int dpl;
    unsigned int p;
    unsigned int limit;
    unsigned int avl;
    unsigned int l;
    unsigned int d;
    unsigned int g;
    unsigned int base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct desc_struct {
    unsigned int a;
    unsigned int b;
    u16 limit0;
    u16 base0;
    unsigned int base1;
    unsigned int type;
    unsigned int s;
    unsigned int dpl;
    unsigned int p;
    unsigned int limit;
    unsigned int avl;
    unsigned int l;
    unsigned int d;
    unsigned int g;
    unsigned int base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct desc_struct {
    unsigned int a;
    unsigned int b;
    u16 limit0;
    u16 base0;
    unsigned int base1;
    unsigned int type;
    unsigned int s;
    unsigned int dpl;
    unsigned int p;
    unsigned int limit;
    unsigned int avl;
    unsigned int l;
    unsigned int d;
    unsigned int g;
    unsigned int base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct desc_struct {
    unsigned int a;
    unsigned int b;
    u16 limit0;
    u16 base0;
    unsigned int base1;
    unsigned int type;
    unsigned int s;
    unsigned int dpl;
    unsigned int p;
    unsigned int limit;
    unsigned int avl;
    unsigned int l;
    unsigned int d;
    unsigned int g;
    unsigned int base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
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
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct desc_struct {
    u16 limit0;
    u16 base0;
    u16 base1;
    u16 type;
    u16 s;
    u16 dpl;
    u16 p;
    u16 limit1;
    u16 avl;
    u16 l;
    u16 d;
    u16 g;
    u16 base2;
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
<code>u16 limit1</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int a</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int b</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int limit</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int base1</code> ➡️ <code>u16 base1</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int type</code> ➡️ <code>u16 type</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int s</code> ➡️ <code>u16 s</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int dpl</code> ➡️ <code>u16 dpl</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int p</code> ➡️ <code>u16 p</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int avl</code> ➡️ <code>u16 avl</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int l</code> ➡️ <code>u16 l</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int d</code> ➡️ <code>u16 d</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int g</code> ➡️ <code>u16 g</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int base2</code> ➡️ <code>u16 base2</code>
</li>
</ul>
</details>
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
