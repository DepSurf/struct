# Struct: <code>fscrypt_mode</code>

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
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    bool logged_impl_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    int logged_impl_name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    int logged_impl_name;
    enum blk_crypto_mode_num blk_crypto_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    int logged_impl_name;
    enum blk_crypto_mode_num blk_crypto_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int security_strength;
    int ivsize;
    int logged_impl_name;
    enum blk_crypto_mode_num blk_crypto_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int security_strength;
    int ivsize;
    int logged_cryptoapi_impl;
    int logged_blk_crypto_native;
    int logged_blk_crypto_fallback;
    enum blk_crypto_mode_num blk_crypto_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int security_strength;
    int ivsize;
    int logged_cryptoapi_impl;
    int logged_blk_crypto_native;
    int logged_blk_crypto_fallback;
    enum blk_crypto_mode_num blk_crypto_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int security_strength;
    int ivsize;
    int logged_cryptoapi_impl;
    int logged_blk_crypto_native;
    int logged_blk_crypto_fallback;
    enum blk_crypto_mode_num blk_crypto_mode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int security_strength;
    int ivsize;
    int logged_cryptoapi_impl;
    int logged_blk_crypto_native;
    int logged_blk_crypto_fallback;
    enum blk_crypto_mode_num blk_crypto_mode;
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
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
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
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fscrypt_mode {
    const char *friendly_name;
    const char *cipher_str;
    int keysize;
    int ivsize;
    bool logged_impl_name;
    bool needs_essiv;
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
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int ivsize</code>
</li>
<li>
<b>Field added. </b>
<code>bool needs_essiv</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>bool needs_essiv</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool logged_impl_name</code> ➡️ <code>int logged_impl_name</code>
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
<code>enum blk_crypto_mode_num blk_crypto_mode</code>
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
<b>Field added. </b>
<code>int security_strength</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int logged_cryptoapi_impl</code>
</li>
<li>
<b>Field added. </b>
<code>int logged_blk_crypto_native</code>
</li>
<li>
<b>Field added. </b>
<code>int logged_blk_crypto_fallback</code>
</li>
<li>
<b>Field removed. </b>
<code>int logged_impl_name</code>
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
