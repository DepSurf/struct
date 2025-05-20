# Struct: <code>ZSTD_matchState_t</code>

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
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
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
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ZSTD_matchState_t {
    ZSTD_window_t window;
    U32 loadedDictEnd;
    U32 nextToUpdate;
    U32 hashLog3;
    U32 *hashTable;
    U32 *hashTable3;
    U32 *chainTable;
    int dedicatedDictSearch;
    optState_t opt;
    const ZSTD_matchState_t *dictMatchState;
    ZSTD_compressionParameters cParams;
    const rawSeqStore_t *ldmSeqStore;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ZSTD_matchState_t {
    ZSTD_window_t window;
    U32 loadedDictEnd;
    U32 nextToUpdate;
    U32 hashLog3;
    U32 rowHashLog;
    U16 *tagTable;
    U32 hashCache[8];
    U32 *hashTable;
    U32 *hashTable3;
    U32 *chainTable;
    U32 forceNonContiguous;
    int dedicatedDictSearch;
    optState_t opt;
    const ZSTD_matchState_t *dictMatchState;
    ZSTD_compressionParameters cParams;
    const rawSeqStore_t *ldmSeqStore;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ZSTD_matchState_t {
    ZSTD_window_t window;
    U32 loadedDictEnd;
    U32 nextToUpdate;
    U32 hashLog3;
    U32 rowHashLog;
    U16 *tagTable;
    U32 hashCache[8];
    U32 *hashTable;
    U32 *hashTable3;
    U32 *chainTable;
    U32 forceNonContiguous;
    int dedicatedDictSearch;
    optState_t opt;
    const ZSTD_matchState_t *dictMatchState;
    ZSTD_compressionParameters cParams;
    const rawSeqStore_t *ldmSeqStore;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ZSTD_matchState_t {
    ZSTD_window_t window;
    U32 loadedDictEnd;
    U32 nextToUpdate;
    U32 hashLog3;
    U32 rowHashLog;
    U16 *tagTable;
    U32 hashCache[8];
    U32 *hashTable;
    U32 *hashTable3;
    U32 *chainTable;
    U32 forceNonContiguous;
    int dedicatedDictSearch;
    optState_t opt;
    const ZSTD_matchState_t *dictMatchState;
    ZSTD_compressionParameters cParams;
    const rawSeqStore_t *ldmSeqStore;
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>U32 rowHashLog</code>
</li>
<li>
<b>Field added. </b>
<code>U16 *tagTable</code>
</li>
<li>
<b>Field added. </b>
<code>U32 hashCache[8]</code>
</li>
<li>
<b>Field added. </b>
<code>U32 forceNonContiguous</code>
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
