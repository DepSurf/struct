# Struct: <code>tcf_pedit</code>

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
In <code>5.0</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    u32 tcfp_off_max_hint;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    struct tcf_pedit_parms *parms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    struct tcf_pedit_parms *parms;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    struct tcf_pedit_parms *parms;
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
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
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
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcf_pedit {
    struct tc_action common;
    unsigned char tcfp_nkeys;
    unsigned char tcfp_flags;
    struct tc_pedit_key *tcfp_keys;
    struct tcf_pedit_key_ex *tcfp_keys_ex;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<code>u32 tcfp_off_max_hint</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tcf_pedit_parms *parms</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char tcfp_nkeys</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned char tcfp_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 tcfp_off_max_hint</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tc_pedit_key *tcfp_keys</code>
</li>
<li>
<b>Field removed. </b>
<code>struct tcf_pedit_key_ex *tcfp_keys_ex</code>
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
