# Struct: <code>skcipher_alg</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_istat_cipher stat;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*export)(struct skcipher_request *, void *);
    int (*import)(struct skcipher_request *, const void *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int walksize;
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int statesize;
    struct crypto_istat_cipher stat;
    struct crypto_alg base;
    struct skcipher_alg_common co;
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
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
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
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct skcipher_alg {
    int (*setkey)(struct crypto_skcipher *, const u8 *, unsigned int);
    int (*encrypt)(struct skcipher_request *);
    int (*decrypt)(struct skcipher_request *);
    int (*init)(struct crypto_skcipher *);
    void (*exit)(struct crypto_skcipher *);
    unsigned int min_keysize;
    unsigned int max_keysize;
    unsigned int ivsize;
    unsigned int chunksize;
    unsigned int walksize;
    struct crypto_alg base;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int walksize</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct crypto_istat_cipher stat</code>
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
<code>int (*export)(struct skcipher_request *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*import)(struct skcipher_request *, const void *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int statesize</code>
</li>
<li>
<b>Field added. </b>
<code>struct skcipher_alg_common co</code>
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
