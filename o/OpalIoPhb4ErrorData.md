# Struct: <code>OpalIoPhb4ErrorData</code>

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
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct OpalIoPhb4ErrorData {
    struct OpalIoPhbErrorCommon common;
    __be32 brdgCtl;
    __be32 deviceStatus;
    __be32 slotStatus;
    __be32 linkStatus;
    __be32 devCmdStatus;
    __be32 devSecStatus;
    __be32 rootErrorStatus;
    __be32 uncorrErrorStatus;
    __be32 corrErrorStatus;
    __be32 tlpHdr1;
    __be32 tlpHdr2;
    __be32 tlpHdr3;
    __be32 tlpHdr4;
    __be32 sourceId;
    __be64 nFir;
    __be64 nFirMask;
    __be64 nFirWOF;
    __be64 phbPlssr;
    __be64 phbCsr;
    __be64 lemFir;
    __be64 lemErrorMask;
    __be64 lemWOF;
    __be64 phbErrorStatus;
    __be64 phbFirstErrorStatus;
    __be64 phbErrorLog0;
    __be64 phbErrorLog1;
    __be64 phbTxeErrorStatus;
    __be64 phbTxeFirstErrorStatus;
    __be64 phbTxeErrorLog0;
    __be64 phbTxeErrorLog1;
    __be64 phbRxeArbErrorStatus;
    __be64 phbRxeArbFirstErrorStatus;
    __be64 phbRxeArbErrorLog0;
    __be64 phbRxeArbErrorLog1;
    __be64 phbRxeMrgErrorStatus;
    __be64 phbRxeMrgFirstErrorStatus;
    __be64 phbRxeMrgErrorLog0;
    __be64 phbRxeMrgErrorLog1;
    __be64 phbRxeTceErrorStatus;
    __be64 phbRxeTceFirstErrorStatus;
    __be64 phbRxeTceErrorLog0;
    __be64 phbRxeTceErrorLog1;
    __be64 phbPblErrorStatus;
    __be64 phbPblFirstErrorStatus;
    __be64 phbPblErrorLog0;
    __be64 phbPblErrorLog1;
    __be64 phbPcieDlpErrorLog1;
    __be64 phbPcieDlpErrorLog2;
    __be64 phbPcieDlpErrorStatus;
    __be64 phbRegbErrorStatus;
    __be64 phbRegbFirstErrorStatus;
    __be64 phbRegbErrorLog0;
    __be64 phbRegbErrorLog1;
    __be64 pestA[512];
    __be64 pestB[512];
};
```
</details>
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
