# Struct: <code>crypto_ahash</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    bool has_setkey;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    bool has_setkey;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    bool has_setkey;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    bool has_setkey;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int statesize;
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct crypto_ahash {
    bool using_shash;
    unsigned int statesize;
    unsigned int reqsize;
    struct crypto_tfm base;
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
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
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
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct crypto_ahash {
    int (*init)(struct ahash_request *);
    int (*update)(struct ahash_request *);
    int (*final)(struct ahash_request *);
    int (*finup)(struct ahash_request *);
    int (*digest)(struct ahash_request *);
    int (*export)(struct ahash_request *, void *);
    int (*import)(struct ahash_request *, const void *);
    int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int);
    unsigned int reqsize;
    struct crypto_tfm base;
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
<b>Field removed. </b>
<code>bool has_setkey</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int statesize</code>
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
<code>bool using_shash</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*init)(struct ahash_request *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*update)(struct ahash_request *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*final)(struct ahash_request *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*finup)(struct ahash_request *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*digest)(struct ahash_request *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*export)(struct ahash_request *, void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*import)(struct ahash_request *, const void *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*setkey)(struct crypto_ahash *, const u8 *, unsigned int)</code>
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
