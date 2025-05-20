# Struct: <code>rctx</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rctx {
    be128 buf[8];
    be128 t;
    be128 *ext;
    struct scatterlist srcbuf[2];
    struct scatterlist dstbuf[2];
    struct scatterlist *src;
    struct scatterlist *dst;
    unsigned int left;
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rctx {
    le128 buf[8];
    le128 t;
    le128 *ext;
    struct scatterlist srcbuf[2];
    struct scatterlist dstbuf[2];
    struct scatterlist *src;
    struct scatterlist *dst;
    unsigned int left;
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rctx {
    le128 buf[8];
    le128 t;
    le128 *ext;
    struct scatterlist srcbuf[2];
    struct scatterlist dstbuf[2];
    struct scatterlist *src;
    struct scatterlist *dst;
    unsigned int left;
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rctx {
    le128 buf[8];
    le128 t;
    le128 *ext;
    struct scatterlist srcbuf[2];
    struct scatterlist dstbuf[2];
    struct scatterlist *src;
    struct scatterlist *dst;
    unsigned int left;
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
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
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
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
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rctx {
    le128 t;
    struct scatterlist *tail;
    struct scatterlist sg[2];
    struct skcipher_request subreq;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>be128 buf[8]</code> ➡️ <code>le128 buf[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>be128 t</code> ➡️ <code>le128 t</code>
</li>
<li>
<b>Field type changed. </b>
<code>be128 *ext</code> ➡️ <code>le128 *ext</code>
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
<b>Field removed. </b>
<code>le128 buf[8]</code>
</li>
<li>
<b>Field removed. </b>
<code>le128 *ext</code>
</li>
<li>
<b>Field removed. </b>
<code>struct scatterlist srcbuf[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct scatterlist dstbuf[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct scatterlist *src</code>
</li>
<li>
<b>Field removed. </b>
<code>struct scatterlist *dst</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int left</code>
</li>
</ul>
</details>
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
<code>struct scatterlist *tail</code>
</li>
<li>
<b>Field added. </b>
<code>struct scatterlist sg[2]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
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
