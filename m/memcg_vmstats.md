# Struct: <code>memcg_vmstats</code>

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
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct memcg_vmstats {
    long int state[42];
    long unsigned int events[98];
    long int state_pending[42];
    long unsigned int events_pending[98];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct memcg_vmstats {
    long int state[42];
    long unsigned int events[100];
    long int state_pending[42];
    long unsigned int events_pending[100];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct memcg_vmstats {
    long int state[48];
    long unsigned int events[107];
    long int state_pending[48];
    long unsigned int events_pending[107];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct memcg_vmstats {
    long int state[50];
    long unsigned int events[19];
    long int state_pending[50];
    long unsigned int events_pending[19];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct memcg_vmstats {
    long int state[50];
    long unsigned int events[19];
    long int state_pending[50];
    long unsigned int events_pending[19];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct memcg_vmstats {
    long int state[53];
    long unsigned int events[22];
    long int state_local[53];
    long unsigned int events_local[22];
    long int state_pending[53];
    long unsigned int events_pending[22];
    atomic64_t stats_updates;
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
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[98]</code> ➡️ <code>long unsigned int events[100]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events_pending[98]</code> ➡️ <code>long unsigned int events_pending[100]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int state[42]</code> ➡️ <code>long int state[48]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[100]</code> ➡️ <code>long unsigned int events[107]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int state_pending[42]</code> ➡️ <code>long int state_pending[48]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events_pending[100]</code> ➡️ <code>long unsigned int events_pending[107]</code>
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
<code>long int state[48]</code> ➡️ <code>long int state[50]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[107]</code> ➡️ <code>long unsigned int events[19]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int state_pending[48]</code> ➡️ <code>long int state_pending[50]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events_pending[107]</code> ➡️ <code>long unsigned int events_pending[19]</code>
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
<b>Field added. </b>
<code>long int state_local[53]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int events_local[22]</code>
</li>
<li>
<b>Field added. </b>
<code>atomic64_t stats_updates</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int state[50]</code> ➡️ <code>long int state[53]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[19]</code> ➡️ <code>long unsigned int events[22]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long int state_pending[50]</code> ➡️ <code>long int state_pending[53]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events_pending[19]</code> ➡️ <code>long unsigned int events_pending[22]</code>
</li>
</ul>
</details>
</li>
</ul>
