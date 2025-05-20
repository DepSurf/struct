# Struct: <code>public_key</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct public_key {
    const struct public_key_algorithm *algo;
    u8 capabilities;
    enum pkey_algo pkey_algo;
    enum pkey_id_type id_type;
    MPI mpi[5];
    struct (anon) dsa;
    struct (anon) rsa;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
    long unsigned int key_eflags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
    long unsigned int key_eflags;
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
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
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
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct public_key {
    void *key;
    u32 keylen;
    enum OID algo;
    void *params;
    u32 paramlen;
    bool key_is_private;
    const char *id_type;
    const char *pkey_algo;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void *key</code>
</li>
<li>
<b>Field added. </b>
<code>u32 keylen</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct public_key_algorithm *algo</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 capabilities</code>
</li>
<li>
<b>Field removed. </b>
<code>MPI mpi[5]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) dsa</code>
</li>
<li>
<b>Field removed. </b>
<code>struct (anon) rsa</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum pkey_algo pkey_algo</code> ➡️ <code>const char *pkey_algo</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum pkey_id_type id_type</code> ➡️ <code>const char *id_type</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool key_is_private</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum OID algo</code>
</li>
<li>
<b>Field added. </b>
<code>void *params</code>
</li>
<li>
<b>Field added. </b>
<code>u32 paramlen</code>
</li>
</ul>
</details>
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
<code>long unsigned int key_eflags</code>
</li>
</ul>
</details>
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
