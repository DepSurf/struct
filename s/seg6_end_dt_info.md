# Struct: <code>seg6_end_dt_info</code>

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
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct seg6_end_dt_info {
    enum seg6_end_dt_mode mode;
    struct net *net;
    int vrf_ifindex;
    int vrf_table;
    __be16 proto;
    u16 family;
    int hdrlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct seg6_end_dt_info {
    enum seg6_end_dt_mode mode;
    struct net *net;
    int vrf_ifindex;
    int vrf_table;
    __be16 proto;
    u16 family;
    int hdrlen;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct seg6_end_dt_info {
    enum seg6_end_dt_mode mode;
    struct net *net;
    int vrf_ifindex;
    int vrf_table;
    u16 family;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct seg6_end_dt_info {
    enum seg6_end_dt_mode mode;
    struct net *net;
    int vrf_ifindex;
    int vrf_table;
    u16 family;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct seg6_end_dt_info {
    enum seg6_end_dt_mode mode;
    struct net *net;
    int vrf_ifindex;
    int vrf_table;
    u16 family;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct seg6_end_dt_info {
    enum seg6_end_dt_mode mode;
    struct net *net;
    int vrf_ifindex;
    int vrf_table;
    u16 family;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct seg6_end_dt_info {
    enum seg6_end_dt_mode mode;
    struct net *net;
    int vrf_ifindex;
    int vrf_table;
    u16 family;
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>__be16 proto</code>
</li>
<li>
<b>Field removed. </b>
<code>int hdrlen</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
