# Struct: <code>mini_Qdisc</code>

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
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    long unsigned int rcu_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    long unsigned int rcu_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    long unsigned int rcu_state;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct tcf_block *block;
    struct gnet_stats_basic_sync *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    long unsigned int rcu_state;
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
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
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
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mini_Qdisc {
    struct tcf_proto *filter_list;
    struct gnet_stats_basic_cpu *cpu_bstats;
    struct gnet_stats_queue *cpu_qstats;
    struct callback_head rcu;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tcf_block *block</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int rcu_state</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head rcu</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct gnet_stats_basic_cpu *cpu_bstats</code> ➡️ <code>struct gnet_stats_basic_sync *cpu_bstats</code>
</li>
</ul>
</details>
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
