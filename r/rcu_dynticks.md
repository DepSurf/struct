# Struct: <code>rcu_dynticks</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct rcu_dynticks {
    long long int dynticks_nesting;
    int dynticks_nmi_nesting;
    atomic_t dynticks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rcu_dynticks {
    long long int dynticks_nesting;
    int dynticks_nmi_nesting;
    atomic_t dynticks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rcu_dynticks {
    long long int dynticks_nesting;
    int dynticks_nmi_nesting;
    atomic_t dynticks;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rcu_dynticks {
    long long int dynticks_nesting;
    int dynticks_nmi_nesting;
    atomic_t dynticks;
    bool rcu_need_heavy_qs;
    long unsigned int rcu_qs_ctr;
    bool rcu_urgent_qs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rcu_dynticks {
    long long int dynticks_nesting;
    int dynticks_nmi_nesting;
    atomic_t dynticks;
    bool rcu_need_heavy_qs;
    long unsigned int rcu_qs_ctr;
    bool rcu_urgent_qs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rcu_dynticks {
    long int dynticks_nesting;
    long int dynticks_nmi_nesting;
    atomic_t dynticks;
    bool rcu_need_heavy_qs;
    long unsigned int rcu_qs_ctr;
    bool rcu_urgent_qs;
};
```
</details>
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool rcu_need_heavy_qs</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int rcu_qs_ctr</code>
</li>
<li>
<b>Field added. </b>
<code>bool rcu_urgent_qs</code>
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
<code>long long int dynticks_nesting</code> ➡️ <code>long int dynticks_nesting</code>
</li>
<li>
<b>Field type changed. </b>
<code>int dynticks_nmi_nesting</code> ➡️ <code>long int dynticks_nmi_nesting</code>
</li>
</ul>
</details>
</li>
</ul>
