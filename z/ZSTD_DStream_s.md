# Struct: <code>ZSTD_DStream_s</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
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
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
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
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ZSTD_DStream_s {
    ZSTD_DCtx *dctx;
    ZSTD_DDict *ddictLocal;
    const ZSTD_DDict *ddict;
    ZSTD_frameParams fParams;
    ZSTD_dStreamStage stage;
    char *inBuff;
    size_t inBuffSize;
    size_t inPos;
    size_t maxWindowSize;
    char *outBuff;
    size_t outBuffSize;
    size_t outStart;
    size_t outEnd;
    size_t blockSize;
    BYTE headerBuffer[18];
    size_t lhSize;
    ZSTD_customMem customMem;
    void *legacyContext;
    U32 previousLegacyVersion;
    U32 legacyVersion;
    U32 hostageByte;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
