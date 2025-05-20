# Struct: <code>shared_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    uint32_t wc_sec_hi;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    uint32_t wc_sec_hi;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    uint32_t wc_sec_hi;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    uint32_t wc_sec_hi;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    uint32_t wc_sec_hi;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    uint32_t wc_sec_hi;
    struct arch_shared_info arch;
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
struct shared_info {
    struct vcpu_info vcpu_info[1];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct shared_info {
    struct vcpu_info vcpu_info[32];
    xen_ulong_t evtchn_pending[64];
    xen_ulong_t evtchn_mask[64];
    struct pvclock_wall_clock wc;
    struct arch_shared_info arch;
};
```
</details>
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>uint32_t wc_sec_hi</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct vcpu_info vcpu_info[32]</code> ➡️ <code>struct vcpu_info vcpu_info[1]</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
