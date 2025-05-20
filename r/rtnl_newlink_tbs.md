# Struct: <code>rtnl_newlink_tbs</code>

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
struct rtnl_newlink_tbs {
    struct nlattr * tb[61];
    struct nlattr * attr[51];
    struct nlattr * slave_attr[41];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rtnl_newlink_tbs {
    struct nlattr * tb[63];
    struct nlattr * attr[51];
    struct nlattr * slave_attr[41];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rtnl_newlink_tbs {
    struct nlattr * tb[65];
    struct nlattr * attr[51];
    struct nlattr * slave_attr[44];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rtnl_newlink_tbs {
    struct nlattr * tb[66];
    struct nlattr * attr[51];
    struct nlattr * slave_attr[45];
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
<b>Field type changed. </b>
<code>struct nlattr * tb[61]</code> ➡️ <code>struct nlattr * tb[63]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct nlattr * tb[63]</code> ➡️ <code>struct nlattr * tb[65]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct nlattr * slave_attr[41]</code> ➡️ <code>struct nlattr * slave_attr[44]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct nlattr * tb[65]</code> ➡️ <code>struct nlattr * tb[66]</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct nlattr * slave_attr[44]</code> ➡️ <code>struct nlattr * slave_attr[45]</code>
</li>
</ul>
</details>
</li>
</ul>
