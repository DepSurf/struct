# Struct: <code>per_cpu_nodestat</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[26];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[26];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[27];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[28];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[30];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[30];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[33];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[38];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[39];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[39];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[41];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[43];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[43];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[46];
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
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
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
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct per_cpu_nodestat {
    s8 stat_threshold;
    s8 vm_node_stat_diff[32];
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[26]</code> ➡️ <code>s8 vm_node_stat_diff[27]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[27]</code> ➡️ <code>s8 vm_node_stat_diff[28]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[28]</code> ➡️ <code>s8 vm_node_stat_diff[30]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[30]</code> ➡️ <code>s8 vm_node_stat_diff[32]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[32]</code> ➡️ <code>s8 vm_node_stat_diff[33]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[33]</code> ➡️ <code>s8 vm_node_stat_diff[38]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[38]</code> ➡️ <code>s8 vm_node_stat_diff[39]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[39]</code> ➡️ <code>s8 vm_node_stat_diff[41]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[41]</code> ➡️ <code>s8 vm_node_stat_diff[43]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>s8 vm_node_stat_diff[43]</code> ➡️ <code>s8 vm_node_stat_diff[46]</code>
</li>
</ul>
</details>
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
