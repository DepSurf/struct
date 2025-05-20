# Struct: <code>ptp_vclock</code>

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
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ptp_vclock {
    struct ptp_clock *pclock;
    struct ptp_clock_info info;
    struct ptp_clock *clock;
    struct cyclecounter cc;
    struct timecounter tc;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ptp_vclock {
    struct ptp_clock *pclock;
    struct ptp_clock_info info;
    struct ptp_clock *clock;
    struct hlist_node vclock_hash_node;
    struct cyclecounter cc;
    struct timecounter tc;
    spinlock_t lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ptp_vclock {
    struct ptp_clock *pclock;
    struct ptp_clock_info info;
    struct ptp_clock *clock;
    struct hlist_node vclock_hash_node;
    struct cyclecounter cc;
    struct timecounter tc;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ptp_vclock {
    struct ptp_clock *pclock;
    struct ptp_clock_info info;
    struct ptp_clock *clock;
    struct hlist_node vclock_hash_node;
    struct cyclecounter cc;
    struct timecounter tc;
    struct mutex lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ptp_vclock {
    struct ptp_clock *pclock;
    struct ptp_clock_info info;
    struct ptp_clock *clock;
    struct hlist_node vclock_hash_node;
    struct cyclecounter cc;
    struct timecounter tc;
    struct mutex lock;
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
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node vclock_hash_node</code>
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
<code>spinlock_t lock</code> ➡️ <code>struct mutex lock</code>
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
