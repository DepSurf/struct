# Struct: <code>kvm_vcpu_stat_generic</code>

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
struct kvm_vcpu_stat_generic {
    u64 halt_successful_poll;
    u64 halt_attempted_poll;
    u64 halt_poll_invalid;
    u64 halt_wakeup;
    u64 halt_poll_success_ns;
    u64 halt_poll_fail_ns;
    u64 halt_wait_ns;
    u64 halt_poll_success_hist[32];
    u64 halt_poll_fail_hist[32];
    u64 halt_wait_hist[32];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_vcpu_stat_generic {
    u64 halt_successful_poll;
    u64 halt_attempted_poll;
    u64 halt_poll_invalid;
    u64 halt_wakeup;
    u64 halt_poll_success_ns;
    u64 halt_poll_fail_ns;
    u64 halt_wait_ns;
    u64 halt_poll_success_hist[32];
    u64 halt_poll_fail_hist[32];
    u64 halt_wait_hist[32];
    u64 blocking;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_vcpu_stat_generic {
    u64 halt_successful_poll;
    u64 halt_attempted_poll;
    u64 halt_poll_invalid;
    u64 halt_wakeup;
    u64 halt_poll_success_ns;
    u64 halt_poll_fail_ns;
    u64 halt_wait_ns;
    u64 halt_poll_success_hist[32];
    u64 halt_poll_fail_hist[32];
    u64 halt_wait_hist[32];
    u64 blocking;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_vcpu_stat_generic {
    u64 halt_successful_poll;
    u64 halt_attempted_poll;
    u64 halt_poll_invalid;
    u64 halt_wakeup;
    u64 halt_poll_success_ns;
    u64 halt_poll_fail_ns;
    u64 halt_wait_ns;
    u64 halt_poll_success_hist[32];
    u64 halt_poll_fail_hist[32];
    u64 halt_wait_hist[32];
    u64 blocking;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_vcpu_stat_generic {
    u64 halt_successful_poll;
    u64 halt_attempted_poll;
    u64 halt_poll_invalid;
    u64 halt_wakeup;
    u64 halt_poll_success_ns;
    u64 halt_poll_fail_ns;
    u64 halt_wait_ns;
    u64 halt_poll_success_hist[32];
    u64 halt_poll_fail_hist[32];
    u64 halt_wait_hist[32];
    u64 blocking;
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
<code>u64 blocking</code>
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
