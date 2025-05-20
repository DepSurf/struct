# Struct: <code>tc_to_netdev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tc_to_netdev {
    unsigned int type;
    u8 tc;
    struct tc_cls_u32_offload *cls_u32;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tc_to_netdev {
    unsigned int type;
    u8 tc;
    struct tc_cls_u32_offload *cls_u32;
    struct tc_cls_flower_offload *cls_flower;
    struct tc_cls_matchall_offload *cls_mall;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tc_to_netdev {
    unsigned int type;
    u8 tc;
    struct tc_cls_u32_offload *cls_u32;
    struct tc_cls_flower_offload *cls_flower;
    struct tc_cls_matchall_offload *cls_mall;
    struct tc_cls_bpf_offload *cls_bpf;
    bool egress_dev;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tc_to_netdev {
    unsigned int type;
    struct tc_cls_u32_offload *cls_u32;
    struct tc_cls_flower_offload *cls_flower;
    struct tc_cls_matchall_offload *cls_mall;
    struct tc_cls_bpf_offload *cls_bpf;
    struct tc_mqprio_qopt *mqprio;
    bool egress_dev;
};
```
</details>
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tc_cls_flower_offload *cls_flower</code>
</li>
<li>
<b>Field added. </b>
<code>struct tc_cls_matchall_offload *cls_mall</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tc_cls_bpf_offload *cls_bpf</code>
</li>
<li>
<b>Field added. </b>
<code>bool egress_dev</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tc_mqprio_qopt *mqprio</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 tc</code>
</li>
</ul>
</details>
</li>
</ul>
