# Struct: <code>nvdimm_security_ops</code>

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
In <code>4.18</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    enum nvdimm_security_state (*state)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    enum nvdimm_security_state (*state)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
    int (*disable_master)(struct nvdimm *, const struct nvdimm_key_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
    int (*disable_master)(struct nvdimm *, const struct nvdimm_key_data *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
    int (*disable_master)(struct nvdimm *, const struct nvdimm_key_data *);
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
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
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
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvdimm_security_ops {
    long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type);
    int (*freeze)(struct nvdimm *);
    int (*change_key)(struct nvdimm *, const struct nvdimm_key_data *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*unlock)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*disable)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*erase)(struct nvdimm *, const struct nvdimm_key_data *, enum nvdimm_passphrase_type);
    int (*overwrite)(struct nvdimm *, const struct nvdimm_key_data *);
    int (*query_overwrite)(struct nvdimm *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int (*get_flags)(struct nvdimm *, enum nvdimm_passphrase_type)</code>
</li>
<li>
<b>Field removed. </b>
<code>enum nvdimm_security_state (*state)(struct nvdimm *, enum nvdimm_passphrase_type)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*disable_master)(struct nvdimm *, const struct nvdimm_key_data *)</code>
</li>
</ul>
</details>
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
