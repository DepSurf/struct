# Struct: <code>cpsw_hw_stats</code>

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
In <code>arm64</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cpsw_hw_stats {
    u32 rxgoodframes;
    u32 rxbroadcastframes;
    u32 rxmulticastframes;
    u32 rxpauseframes;
    u32 rxcrcerrors;
    u32 rxaligncodeerrors;
    u32 rxoversizedframes;
    u32 rxjabberframes;
    u32 rxundersizedframes;
    u32 rxfragments;
    u32 __pad_0[2];
    u32 rxoctets;
    u32 txgoodframes;
    u32 txbroadcastframes;
    u32 txmulticastframes;
    u32 txpauseframes;
    u32 txdeferredframes;
    u32 txcollisionframes;
    u32 txsinglecollframes;
    u32 txmultcollframes;
    u32 txexcessivecollisions;
    u32 txlatecollisions;
    u32 txunderrun;
    u32 txcarriersenseerrors;
    u32 txoctets;
    u32 octetframes64;
    u32 octetframes65t127;
    u32 octetframes128t255;
    u32 octetframes256t511;
    u32 octetframes512t1023;
    u32 octetframes1024tup;
    u32 netoctets;
    u32 rxsofoverruns;
    u32 rxmofoverruns;
    u32 rxdmaoverruns;
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
