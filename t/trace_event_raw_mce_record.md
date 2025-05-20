# Struct: <code>trace_event_raw_mce_record</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
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
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct trace_event_raw_mce_record {
    struct trace_entry ent;
    u64 mcgcap;
    u64 mcgstatus;
    u64 status;
    u64 addr;
    u64 misc;
    u64 synd;
    u64 ipid;
    u64 ip;
    u64 tsc;
    u64 walltime;
    u32 cpu;
    u32 cpuid;
    u32 apicid;
    u32 socketid;
    u8 cs;
    u8 bank;
    u8 cpuvendor;
    char __data[0];
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 synd</code>
</li>
<li>
<b>Field added. </b>
<code>u64 ipid</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
