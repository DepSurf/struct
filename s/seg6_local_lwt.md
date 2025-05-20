# Struct: <code>seg6_local_lwt</code>

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
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    struct seg6_end_dt_info dt_info;
    int headroom;
    struct seg6_action_desc *desc;
    long unsigned int parsed_optattrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    struct seg6_end_dt_info dt_info;
    struct pcpu_seg6_local_counters *pcpu_counters;
    int headroom;
    struct seg6_action_desc *desc;
    long unsigned int parsed_optattrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    struct seg6_end_dt_info dt_info;
    struct pcpu_seg6_local_counters *pcpu_counters;
    int headroom;
    struct seg6_action_desc *desc;
    long unsigned int parsed_optattrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    struct seg6_end_dt_info dt_info;
    struct pcpu_seg6_local_counters *pcpu_counters;
    int headroom;
    struct seg6_action_desc *desc;
    long unsigned int parsed_optattrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    struct seg6_end_dt_info dt_info;
    struct seg6_flavors_info flv_info;
    struct pcpu_seg6_local_counters *pcpu_counters;
    int headroom;
    struct seg6_action_desc *desc;
    long unsigned int parsed_optattrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    struct seg6_end_dt_info dt_info;
    struct seg6_flavors_info flv_info;
    struct pcpu_seg6_local_counters *pcpu_counters;
    int headroom;
    struct seg6_action_desc *desc;
    long unsigned int parsed_optattrs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    struct seg6_end_dt_info dt_info;
    struct seg6_flavors_info flv_info;
    struct pcpu_seg6_local_counters *pcpu_counters;
    int headroom;
    struct seg6_action_desc *desc;
    long unsigned int parsed_optattrs;
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
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
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
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct seg6_local_lwt {
    int action;
    struct ipv6_sr_hdr *srh;
    int table;
    struct in_addr nh4;
    struct in6_addr nh6;
    int iif;
    int oif;
    struct bpf_lwt_prog bpf;
    int headroom;
    struct seg6_action_desc *desc;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct bpf_lwt_prog bpf</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct seg6_end_dt_info dt_info</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int parsed_optattrs</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct pcpu_seg6_local_counters *pcpu_counters</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct seg6_flavors_info flv_info</code>
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
