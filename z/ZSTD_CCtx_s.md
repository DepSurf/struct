# Struct: <code>ZSTD_CCtx_s</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ZSTD_CCtx_s {
    const BYTE *nextSrc;
    const BYTE *base;
    const BYTE *dictBase;
    U32 dictLimit;
    U32 lowLimit;
    U32 nextToUpdate;
    U32 nextToUpdate3;
    U32 hashLog3;
    U32 loadedDictEnd;
    U32 forceWindow;
    U32 forceRawDict;
    ZSTD_compressionStage_e stage;
    U32 rep[3];
    U32 repToConfirm[3];
    U32 dictID;
    ZSTD_parameters params;
    void *workSpace;
    size_t workSpaceSize;
    size_t blockSize;
    U64 frameContentSize;
    struct xxh64_state xxhState;
    ZSTD_customMem customMem;
    seqStore_t seqStore;
    U32 *hashTable;
    U32 *hashTable3;
    U32 *chainTable;
    HUF_CElt *hufTable;
    U32 flagStaticTables;
    HUF_repeat flagStaticHufTable;
    FSE_CTable offcodeCTable[187];
    FSE_CTable matchlengthCTable[363];
    FSE_CTable litlengthCTable[329];
    unsigned int tmpCounters[1536];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ZSTD_CCtx_s {
    const BYTE *nextSrc;
    const BYTE *base;
    const BYTE *dictBase;
    U32 dictLimit;
    U32 lowLimit;
    U32 nextToUpdate;
    U32 nextToUpdate3;
    U32 hashLog3;
    U32 loadedDictEnd;
    U32 forceWindow;
    U32 forceRawDict;
    ZSTD_compressionStage_e stage;
    U32 rep[3];
    U32 repToConfirm[3];
    U32 dictID;
    ZSTD_parameters params;
    void *workSpace;
    size_t workSpaceSize;
    size_t blockSize;
    U64 frameContentSize;
    struct xxh64_state xxhState;
    ZSTD_customMem customMem;
    seqStore_t seqStore;
    U32 *hashTable;
    U32 *hashTable3;
    U32 *chainTable;
    HUF_CElt *hufTable;
    U32 flagStaticTables;
    HUF_repeat flagStaticHufTable;
    FSE_CTable offcodeCTable[187];
    FSE_CTable matchlengthCTable[363];
    FSE_CTable litlengthCTable[329];
    unsigned int tmpCounters[1536];
};
```
</details>
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
struct ZSTD_CCtx_s {
    ZSTD_compressionStage_e stage;
    int cParamsChanged;
    int bmi2;
    ZSTD_CCtx_params requestedParams;
    ZSTD_CCtx_params appliedParams;
    U32 dictID;
    size_t dictContentSize;
    ZSTD_cwksp workspace;
    size_t blockSize;
    long long unsigned int pledgedSrcSizePlusOne;
    long long unsigned int consumedSrcSize;
    long long unsigned int producedCSize;
    struct xxh64_state xxhState;
    ZSTD_customMem customMem;
    ZSTD_threadPool *pool;
    size_t staticSize;
    SeqCollector seqCollector;
    int isFirstBlock;
    int initialized;
    seqStore_t seqStore;
    ldmState_t ldmState;
    rawSeq *ldmSequences;
    size_t maxNbLdmSequences;
    rawSeqStore_t externSeqStore;
    ZSTD_blockState_t blockState;
    U32 *entropyWorkspace;
    ZSTD_buffered_policy_e bufferedPolicy;
    char *inBuff;
    size_t inBuffSize;
    size_t inToCompress;
    size_t inBuffPos;
    size_t inBuffTarget;
    char *outBuff;
    size_t outBuffSize;
    size_t outBuffContentSize;
    size_t outBuffFlushedSize;
    ZSTD_cStreamStage streamStage;
    U32 frameEnded;
    ZSTD_inBuffer expectedInBuffer;
    size_t expectedOutBufferSize;
    ZSTD_localDict localDict;
    const ZSTD_CDict *cdict;
    ZSTD_prefixDict prefixDict;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ZSTD_CCtx_s {
    ZSTD_compressionStage_e stage;
    int cParamsChanged;
    int bmi2;
    ZSTD_CCtx_params requestedParams;
    ZSTD_CCtx_params appliedParams;
    ZSTD_CCtx_params simpleApiParams;
    U32 dictID;
    size_t dictContentSize;
    ZSTD_cwksp workspace;
    size_t blockSize;
    long long unsigned int pledgedSrcSizePlusOne;
    long long unsigned int consumedSrcSize;
    long long unsigned int producedCSize;
    struct xxh64_state xxhState;
    ZSTD_customMem customMem;
    ZSTD_threadPool *pool;
    size_t staticSize;
    SeqCollector seqCollector;
    int isFirstBlock;
    int initialized;
    seqStore_t seqStore;
    ldmState_t ldmState;
    rawSeq *ldmSequences;
    size_t maxNbLdmSequences;
    rawSeqStore_t externSeqStore;
    ZSTD_blockState_t blockState;
    U32 *entropyWorkspace;
    ZSTD_buffered_policy_e bufferedPolicy;
    char *inBuff;
    size_t inBuffSize;
    size_t inToCompress;
    size_t inBuffPos;
    size_t inBuffTarget;
    char *outBuff;
    size_t outBuffSize;
    size_t outBuffContentSize;
    size_t outBuffFlushedSize;
    ZSTD_cStreamStage streamStage;
    U32 frameEnded;
    ZSTD_inBuffer expectedInBuffer;
    size_t expectedOutBufferSize;
    ZSTD_localDict localDict;
    const ZSTD_CDict *cdict;
    ZSTD_prefixDict prefixDict;
    ZSTD_blockSplitCtx blockSplitCtx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ZSTD_CCtx_s {
    ZSTD_compressionStage_e stage;
    int cParamsChanged;
    int bmi2;
    ZSTD_CCtx_params requestedParams;
    ZSTD_CCtx_params appliedParams;
    ZSTD_CCtx_params simpleApiParams;
    U32 dictID;
    size_t dictContentSize;
    ZSTD_cwksp workspace;
    size_t blockSize;
    long long unsigned int pledgedSrcSizePlusOne;
    long long unsigned int consumedSrcSize;
    long long unsigned int producedCSize;
    struct xxh64_state xxhState;
    ZSTD_customMem customMem;
    ZSTD_threadPool *pool;
    size_t staticSize;
    SeqCollector seqCollector;
    int isFirstBlock;
    int initialized;
    seqStore_t seqStore;
    ldmState_t ldmState;
    rawSeq *ldmSequences;
    size_t maxNbLdmSequences;
    rawSeqStore_t externSeqStore;
    ZSTD_blockState_t blockState;
    U32 *entropyWorkspace;
    ZSTD_buffered_policy_e bufferedPolicy;
    char *inBuff;
    size_t inBuffSize;
    size_t inToCompress;
    size_t inBuffPos;
    size_t inBuffTarget;
    char *outBuff;
    size_t outBuffSize;
    size_t outBuffContentSize;
    size_t outBuffFlushedSize;
    ZSTD_cStreamStage streamStage;
    U32 frameEnded;
    ZSTD_inBuffer expectedInBuffer;
    size_t expectedOutBufferSize;
    ZSTD_localDict localDict;
    const ZSTD_CDict *cdict;
    ZSTD_prefixDict prefixDict;
    ZSTD_blockSplitCtx blockSplitCtx;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ZSTD_CCtx_s {
    ZSTD_compressionStage_e stage;
    int cParamsChanged;
    int bmi2;
    ZSTD_CCtx_params requestedParams;
    ZSTD_CCtx_params appliedParams;
    ZSTD_CCtx_params simpleApiParams;
    U32 dictID;
    size_t dictContentSize;
    ZSTD_cwksp workspace;
    size_t blockSize;
    long long unsigned int pledgedSrcSizePlusOne;
    long long unsigned int consumedSrcSize;
    long long unsigned int producedCSize;
    struct xxh64_state xxhState;
    ZSTD_customMem customMem;
    ZSTD_threadPool *pool;
    size_t staticSize;
    SeqCollector seqCollector;
    int isFirstBlock;
    int initialized;
    seqStore_t seqStore;
    ldmState_t ldmState;
    rawSeq *ldmSequences;
    size_t maxNbLdmSequences;
    rawSeqStore_t externSeqStore;
    ZSTD_blockState_t blockState;
    U32 *entropyWorkspace;
    ZSTD_buffered_policy_e bufferedPolicy;
    char *inBuff;
    size_t inBuffSize;
    size_t inToCompress;
    size_t inBuffPos;
    size_t inBuffTarget;
    char *outBuff;
    size_t outBuffSize;
    size_t outBuffContentSize;
    size_t outBuffFlushedSize;
    ZSTD_cStreamStage streamStage;
    U32 frameEnded;
    ZSTD_inBuffer expectedInBuffer;
    size_t expectedOutBufferSize;
    ZSTD_localDict localDict;
    const ZSTD_CDict *cdict;
    ZSTD_prefixDict prefixDict;
    ZSTD_blockSplitCtx blockSplitCtx;
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
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>ZSTD_CCtx_params simpleApiParams</code>
</li>
<li>
<b>Field added. </b>
<code>ZSTD_blockSplitCtx blockSplitCtx</code>
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
