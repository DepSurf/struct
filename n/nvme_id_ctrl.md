# Struct: <code>nvme_id_ctrl</code>

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
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct nvme_id_ctrl {
    __le16 vid;
    __le16 ssvid;
    char sn[20];
    char mn[40];
    char fr[8];
    __u8 rab;
    __u8 ieee[3];
    __u8 cmic;
    __u8 mdts;
    __le16 cntlid;
    __le32 ver;
    __le32 rtd3r;
    __le32 rtd3e;
    __le32 oaes;
    __le32 ctratt;
    __u8 rsvd100[28];
    __le16 crdt1;
    __le16 crdt2;
    __le16 crdt3;
    __u8 rsvd134[122];
    __le16 oacs;
    __u8 acl;
    __u8 aerl;
    __u8 frmw;
    __u8 lpa;
    __u8 elpe;
    __u8 npss;
    __u8 avscc;
    __u8 apsta;
    __le16 wctemp;
    __le16 cctemp;
    __le16 mtfa;
    __le32 hmpre;
    __le32 hmmin;
    __u8 tnvmcap[16];
    __u8 unvmcap[16];
    __le32 rpmbs;
    __le16 edstt;
    __u8 dsto;
    __u8 fwug;
    __le16 kas;
    __le16 hctma;
    __le16 mntmt;
    __le16 mxtmt;
    __le32 sanicap;
    __le32 hmminds;
    __le16 hmmaxd;
    __u8 rsvd338[4];
    __u8 anatt;
    __u8 anacap;
    __le32 anagrpmax;
    __le32 nanagrpid;
    __u8 rsvd352[160];
    __u8 sqes;
    __u8 cqes;
    __le16 maxcmd;
    __le32 nn;
    __le16 oncs;
    __le16 fuses;
    __u8 fna;
    __u8 vwc;
    __le16 awun;
    __le16 awupf;
    __u8 nvscc;
    __u8 nwpc;
    __le16 acwu;
    __u8 rsvd534[2];
    __le32 sgls;
    __le32 mnan;
    __u8 rsvd544[224];
    char subnqn[256];
    __u8 rsvd1024[768];
    __le32 ioccsz;
    __le32 iorcsz;
    __le16 icdoff;
    __u8 ctrattr;
    __u8 msdbd;
    __u8 rsvd1804[244];
    struct nvme_id_power_state psd[32];
    __u8 vs[1024];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvme_id_ctrl {
    __le16 vid;
    __le16 ssvid;
    char sn[20];
    char mn[40];
    char fr[8];
    __u8 rab;
    __u8 ieee[3];
    __u8 cmic;
    __u8 mdts;
    __le16 cntlid;
    __le32 ver;
    __le32 rtd3r;
    __le32 rtd3e;
    __le32 oaes;
    __le32 ctratt;
    __u8 rsvd100[28];
    __le16 crdt1;
    __le16 crdt2;
    __le16 crdt3;
    __u8 rsvd134[122];
    __le16 oacs;
    __u8 acl;
    __u8 aerl;
    __u8 frmw;
    __u8 lpa;
    __u8 elpe;
    __u8 npss;
    __u8 avscc;
    __u8 apsta;
    __le16 wctemp;
    __le16 cctemp;
    __le16 mtfa;
    __le32 hmpre;
    __le32 hmmin;
    __u8 tnvmcap[16];
    __u8 unvmcap[16];
    __le32 rpmbs;
    __le16 edstt;
    __u8 dsto;
    __u8 fwug;
    __le16 kas;
    __le16 hctma;
    __le16 mntmt;
    __le16 mxtmt;
    __le32 sanicap;
    __le32 hmminds;
    __le16 hmmaxd;
    __u8 rsvd338[4];
    __u8 anatt;
    __u8 anacap;
    __le32 anagrpmax;
    __le32 nanagrpid;
    __u8 rsvd352[160];
    __u8 sqes;
    __u8 cqes;
    __le16 maxcmd;
    __le32 nn;
    __le16 oncs;
    __le16 fuses;
    __u8 fna;
    __u8 vwc;
    __le16 awun;
    __le16 awupf;
    __u8 nvscc;
    __u8 nwpc;
    __le16 acwu;
    __u8 rsvd534[2];
    __le32 sgls;
    __le32 mnan;
    __u8 rsvd544[224];
    char subnqn[256];
    __u8 rsvd1024[768];
    __le32 ioccsz;
    __le32 iorcsz;
    __le16 icdoff;
    __u8 ctrattr;
    __u8 msdbd;
    __u8 rsvd1804[244];
    struct nvme_id_power_state psd[32];
    __u8 vs[1024];
};
```
</details>
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Flavor</b>
<ul>
</ul>
