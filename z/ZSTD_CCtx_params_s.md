# Struct: <code>ZSTD_CCtx_params_s</code>

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
struct ZSTD_CCtx_params_s {
    ZSTD_format_e format;
    ZSTD_compressionParameters cParams;
    ZSTD_frameParameters fParams;
    int compressionLevel;
    int forceWindow;
    size_t targetCBlockSize;
    int srcSizeHint;
    ZSTD_dictAttachPref_e attachDictPref;
    ZSTD_literalCompressionMode_e literalCompressionMode;
    int nbWorkers;
    size_t jobSize;
    int overlapLog;
    int rsyncable;
    ldmParams_t ldmParams;
    int enableDedicatedDictSearch;
    ZSTD_bufferMode_e inBufferMode;
    ZSTD_bufferMode_e outBufferMode;
    ZSTD_sequenceFormat_e blockDelimiters;
    int validateSequences;
    ZSTD_customMem customMem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ZSTD_CCtx_params_s {
    ZSTD_format_e format;
    ZSTD_compressionParameters cParams;
    ZSTD_frameParameters fParams;
    int compressionLevel;
    int forceWindow;
    size_t targetCBlockSize;
    int srcSizeHint;
    ZSTD_dictAttachPref_e attachDictPref;
    ZSTD_paramSwitch_e literalCompressionMode;
    int nbWorkers;
    size_t jobSize;
    int overlapLog;
    int rsyncable;
    ldmParams_t ldmParams;
    int enableDedicatedDictSearch;
    ZSTD_bufferMode_e inBufferMode;
    ZSTD_bufferMode_e outBufferMode;
    ZSTD_sequenceFormat_e blockDelimiters;
    int validateSequences;
    ZSTD_paramSwitch_e useBlockSplitter;
    ZSTD_paramSwitch_e useRowMatchFinder;
    int deterministicRefPrefix;
    ZSTD_customMem customMem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ZSTD_CCtx_params_s {
    ZSTD_format_e format;
    ZSTD_compressionParameters cParams;
    ZSTD_frameParameters fParams;
    int compressionLevel;
    int forceWindow;
    size_t targetCBlockSize;
    int srcSizeHint;
    ZSTD_dictAttachPref_e attachDictPref;
    ZSTD_paramSwitch_e literalCompressionMode;
    int nbWorkers;
    size_t jobSize;
    int overlapLog;
    int rsyncable;
    ldmParams_t ldmParams;
    int enableDedicatedDictSearch;
    ZSTD_bufferMode_e inBufferMode;
    ZSTD_bufferMode_e outBufferMode;
    ZSTD_sequenceFormat_e blockDelimiters;
    int validateSequences;
    ZSTD_paramSwitch_e useBlockSplitter;
    ZSTD_paramSwitch_e useRowMatchFinder;
    int deterministicRefPrefix;
    ZSTD_customMem customMem;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ZSTD_CCtx_params_s {
    ZSTD_format_e format;
    ZSTD_compressionParameters cParams;
    ZSTD_frameParameters fParams;
    int compressionLevel;
    int forceWindow;
    size_t targetCBlockSize;
    int srcSizeHint;
    ZSTD_dictAttachPref_e attachDictPref;
    ZSTD_paramSwitch_e literalCompressionMode;
    int nbWorkers;
    size_t jobSize;
    int overlapLog;
    int rsyncable;
    ldmParams_t ldmParams;
    int enableDedicatedDictSearch;
    ZSTD_bufferMode_e inBufferMode;
    ZSTD_bufferMode_e outBufferMode;
    ZSTD_sequenceFormat_e blockDelimiters;
    int validateSequences;
    ZSTD_paramSwitch_e useBlockSplitter;
    ZSTD_paramSwitch_e useRowMatchFinder;
    int deterministicRefPrefix;
    ZSTD_customMem customMem;
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
<code>ZSTD_paramSwitch_e useBlockSplitter</code>
</li>
<li>
<b>Field added. </b>
<code>ZSTD_paramSwitch_e useRowMatchFinder</code>
</li>
<li>
<b>Field added. </b>
<code>int deterministicRefPrefix</code>
</li>
<li>
<b>Field type changed. </b>
<code>ZSTD_literalCompressionMode_e literalCompressionMode</code> ➡️ <code>ZSTD_paramSwitch_e literalCompressionMode</code>
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
