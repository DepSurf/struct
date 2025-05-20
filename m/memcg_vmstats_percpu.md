# Struct: <code>memcg_vmstats_percpu</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[36];
    long unsigned int events[85];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[85];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[36];
    long unsigned int events[92];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[41];
    long unsigned int events[96];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int state[42];
    long unsigned int events[98];
    long int state_prev[42];
    long unsigned int events_prev[98];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int state[42];
    long unsigned int events[100];
    long int state_prev[42];
    long unsigned int events_prev[100];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int state[48];
    long unsigned int events[107];
    long int state_prev[48];
    long unsigned int events_prev[107];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int state[50];
    long unsigned int events[19];
    long int state_prev[50];
    long unsigned int events_prev[19];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int state[50];
    long unsigned int events[19];
    long int state_prev[50];
    long unsigned int events_prev[19];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    unsigned int stats_updates;
    struct memcg_vmstats_percpu *parent;
    struct memcg_vmstats *vmstats;
    long int state[53];
    long unsigned int events[22];
    long int state_prev[53];
    long unsigned int events_prev[22];
    long unsigned int nr_page_events;
    long unsigned int targets[2];
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
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[81];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[59];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[78];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[61];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
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
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[85];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[85];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[85];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct memcg_vmstats_percpu {
    long int stat[38];
    long unsigned int events[85];
    long unsigned int nr_page_events;
    long unsigned int targets[3];
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
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long int stat[36]</code> ➡️ <code>long int stat[38]</code>
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
<code>long int stat[38]</code> ➡️ <code>long int stat[36]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[85]</code> ➡️ <code>long unsigned int events[92]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int targets[3]</code> ➡️ <code>long unsigned int targets[2]</code>
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
<code>long int stat[36]</code> ➡️ <code>long int stat[41]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[92]</code> ➡️ <code>long unsigned int events[96]</code>
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
<code>long int state[42]</code>
</li>
<li>
<b>Field added. </b>
<code>long int state_prev[42]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int events_prev[98]</code>
</li>
<li>
<b>Field removed. </b>
<code>long int stat[41]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[96]</code> ➡️ <code>long unsigned int events[98]</code>
</li>
</ul>
</details>
</li>
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
<code>long unsigned int events_prev[98]</code> ➡️ <code>long unsigned int events_prev[100]</code>
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
<code>long int state_prev[42]</code> ➡️ <code>long int state_prev[48]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events_prev[100]</code> ➡️ <code>long unsigned int events_prev[107]</code>
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
<code>long int state_prev[48]</code> ➡️ <code>long int state_prev[50]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events_prev[107]</code> ➡️ <code>long unsigned int events_prev[19]</code>
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
<code>unsigned int stats_updates</code>
</li>
<li>
<b>Field added. </b>
<code>struct memcg_vmstats_percpu *parent</code>
</li>
<li>
<b>Field added. </b>
<code>struct memcg_vmstats *vmstats</code>
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
<code>long int state_prev[50]</code> ➡️ <code>long int state_prev[53]</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int events_prev[19]</code> ➡️ <code>long unsigned int events_prev[22]</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[85]</code> ➡️ <code>long unsigned int events[81]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[85]</code> ➡️ <code>long unsigned int events[59]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>ppc64el</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[85]</code> ➡️ <code>long unsigned int events[78]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>long unsigned int events[85]</code> ➡️ <code>long unsigned int events[61]</code>
</li>
</ul>
</details>
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
