# Struct: <code>xen_mce</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
    __u64 synd;
    __u64 ipid;
    __u64 ppin;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
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
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xen_mce {
    __u64 status;
    __u64 misc;
    __u64 addr;
    __u64 mcgstatus;
    __u64 ip;
    __u64 tsc;
    __u64 time;
    __u8 cpuvendor;
    __u8 inject_flags;
    __u16 pad;
    __u32 cpuid;
    __u8 cs;
    __u8 bank;
    __u8 cpu;
    __u8 finished;
    __u32 extcpu;
    __u32 socketid;
    __u32 apicid;
    __u64 mcgcap;
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u64 synd</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 ipid</code>
</li>
<li>
<b>Field added. </b>
<code>__u64 ppin</code>
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
