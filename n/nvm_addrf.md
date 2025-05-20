# Struct: <code>nvm_addrf</code>

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
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
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
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
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
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvm_addrf {
    u8 ch_len;
    u8 lun_len;
    u8 chk_len;
    u8 sec_len;
    u8 rsv_len[2];
    u8 ch_offset;
    u8 lun_offset;
    u8 chk_offset;
    u8 sec_offset;
    u8 rsv_off[2];
    u64 ch_mask;
    u64 lun_mask;
    u64 chk_mask;
    u64 sec_mask;
    u64 rsv_mask[2];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
