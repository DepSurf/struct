# Struct: <code>ptc_stats</code>

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
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ptc_stats {
    long unsigned int s_giveup;
    long unsigned int s_requestor;
    long unsigned int s_stimeout;
    long unsigned int s_dtimeout;
    long unsigned int s_strongnacks;
    long unsigned int s_time;
    long unsigned int s_retriesok;
    long unsigned int s_ntargcpu;
    long unsigned int s_ntargself;
    long unsigned int s_ntarglocals;
    long unsigned int s_ntargremotes;
    long unsigned int s_ntarglocaluvhub;
    long unsigned int s_ntargremoteuvhub;
    long unsigned int s_ntarguvhub;
    long unsigned int s_ntarguvhub16;
    long unsigned int s_ntarguvhub8;
    long unsigned int s_ntarguvhub4;
    long unsigned int s_ntarguvhub2;
    long unsigned int s_ntarguvhub1;
    long unsigned int s_resets_plug;
    long unsigned int s_resets_timeout;
    long unsigned int s_busy;
    long unsigned int s_throttles;
    long unsigned int s_retry_messages;
    long unsigned int s_bau_reenabled;
    long unsigned int s_bau_disabled;
    long unsigned int s_uv2_wars;
    long unsigned int s_uv2_wars_hw;
    long unsigned int s_uv2_war_waits;
    long unsigned int s_overipilimit;
    long unsigned int s_giveuplimit;
    long unsigned int s_enters;
    long unsigned int s_ipifordisabled;
    long unsigned int s_plugged;
    long unsigned int s_congested;
    long unsigned int d_alltlb;
    long unsigned int d_onetlb;
    long unsigned int d_multmsg;
    long unsigned int d_nomsg;
    long unsigned int d_time;
    long unsigned int d_requestee;
    long unsigned int d_retries;
    long unsigned int d_canceled;
    long unsigned int d_nocanceled;
    long unsigned int d_resets;
    long unsigned int d_rcanceled;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ptc_stats {
    long unsigned int s_giveup;
    long unsigned int s_requestor;
    long unsigned int s_stimeout;
    long unsigned int s_dtimeout;
    long unsigned int s_strongnacks;
    long unsigned int s_time;
    long unsigned int s_retriesok;
    long unsigned int s_ntargcpu;
    long unsigned int s_ntargself;
    long unsigned int s_ntarglocals;
    long unsigned int s_ntargremotes;
    long unsigned int s_ntarglocaluvhub;
    long unsigned int s_ntargremoteuvhub;
    long unsigned int s_ntarguvhub;
    long unsigned int s_ntarguvhub16;
    long unsigned int s_ntarguvhub8;
    long unsigned int s_ntarguvhub4;
    long unsigned int s_ntarguvhub2;
    long unsigned int s_ntarguvhub1;
    long unsigned int s_resets_plug;
    long unsigned int s_resets_timeout;
    long unsigned int s_busy;
    long unsigned int s_throttles;
    long unsigned int s_retry_messages;
    long unsigned int s_bau_reenabled;
    long unsigned int s_bau_disabled;
    long unsigned int s_uv2_wars;
    long unsigned int s_uv2_wars_hw;
    long unsigned int s_uv2_war_waits;
    long unsigned int s_overipilimit;
    long unsigned int s_giveuplimit;
    long unsigned int s_enters;
    long unsigned int s_ipifordisabled;
    long unsigned int s_plugged;
    long unsigned int s_congested;
    long unsigned int d_alltlb;
    long unsigned int d_onetlb;
    long unsigned int d_multmsg;
    long unsigned int d_nomsg;
    long unsigned int d_time;
    long unsigned int d_requestee;
    long unsigned int d_retries;
    long unsigned int d_canceled;
    long unsigned int d_nocanceled;
    long unsigned int d_resets;
    long unsigned int d_rcanceled;
};
```
</details>
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ptc_stats {
    long unsigned int s_giveup;
    long unsigned int s_requestor;
    long unsigned int s_stimeout;
    long unsigned int s_dtimeout;
    long unsigned int s_strongnacks;
    long unsigned int s_time;
    long unsigned int s_retriesok;
    long unsigned int s_ntargcpu;
    long unsigned int s_ntargself;
    long unsigned int s_ntarglocals;
    long unsigned int s_ntargremotes;
    long unsigned int s_ntarglocaluvhub;
    long unsigned int s_ntargremoteuvhub;
    long unsigned int s_ntarguvhub;
    long unsigned int s_ntarguvhub16;
    long unsigned int s_ntarguvhub8;
    long unsigned int s_ntarguvhub4;
    long unsigned int s_ntarguvhub2;
    long unsigned int s_ntarguvhub1;
    long unsigned int s_resets_plug;
    long unsigned int s_resets_timeout;
    long unsigned int s_busy;
    long unsigned int s_throttles;
    long unsigned int s_retry_messages;
    long unsigned int s_bau_reenabled;
    long unsigned int s_bau_disabled;
    long unsigned int s_uv2_wars;
    long unsigned int s_uv2_wars_hw;
    long unsigned int s_uv2_war_waits;
    long unsigned int s_overipilimit;
    long unsigned int s_giveuplimit;
    long unsigned int s_enters;
    long unsigned int s_ipifordisabled;
    long unsigned int s_plugged;
    long unsigned int s_congested;
    long unsigned int d_alltlb;
    long unsigned int d_onetlb;
    long unsigned int d_multmsg;
    long unsigned int d_nomsg;
    long unsigned int d_time;
    long unsigned int d_requestee;
    long unsigned int d_retries;
    long unsigned int d_canceled;
    long unsigned int d_nocanceled;
    long unsigned int d_resets;
    long unsigned int d_rcanceled;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
