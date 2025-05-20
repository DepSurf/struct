# Struct: <code>cpuinfo_x86</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_mask;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[17];
    char x86_vendor_id[16];
    char x86_model_id[64];
    int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u8 compute_unit_id;
    u16 cpu_index;
    u32 microcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_mask;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[19];
    char x86_vendor_id[16];
    char x86_model_id[64];
    int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_index;
    u32 microcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_mask;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[19];
    char x86_vendor_id[16];
    char x86_model_id[64];
    int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_index;
    u32 microcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_mask;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[19];
    char x86_vendor_id[16];
    char x86_model_id[64];
    int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_index;
    u32 microcode;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_index;
    u32 microcode;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[3];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[3];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[3];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[21];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[3];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[21];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    bool smt_active;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[3];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[21];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u64 ppin;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    bool smt_active;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[5];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[21];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u64 ppin;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    bool smt_active;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[5];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[23];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u64 ppin;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    bool smt_active;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u32 vmx_capability[5];
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[24];
    long unsigned int x86_capability_alignment;
    char x86_vendor_id[16];
    char x86_model_id[64];
    struct cpuinfo_topology topo;
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_cache_mbm_width_offset;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u64 ppin;
    u16 x86_max_cores;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 cpu_index;
    bool smt_active;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
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
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cpuinfo_x86 {
    __u8 x86;
    __u8 x86_vendor;
    __u8 x86_model;
    __u8 x86_stepping;
    int x86_tlbsize;
    __u8 x86_virt_bits;
    __u8 x86_phys_bits;
    __u8 x86_coreid_bits;
    __u8 cu_id;
    __u32 extended_cpuid_level;
    int cpuid_level;
    __u32 x86_capability[20];
    char x86_vendor_id[16];
    char x86_model_id[64];
    unsigned int x86_cache_size;
    int x86_cache_alignment;
    int x86_cache_max_rmid;
    int x86_cache_occ_scale;
    int x86_power;
    long unsigned int loops_per_jiffy;
    u16 x86_max_cores;
    u16 apicid;
    u16 initial_apicid;
    u16 x86_clflush_size;
    u16 booted_cores;
    u16 phys_proc_id;
    u16 logical_proc_id;
    u16 cpu_core_id;
    u16 cpu_die_id;
    u16 logical_die_id;
    u16 cpu_index;
    u32 microcode;
    u8 x86_cache_bits;
    unsigned int initialized;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u8 compute_unit_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 x86_capability[17]</code> ➡️ <code>__u32 x86_capability[19]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 cu_id</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>__u8 x86_stepping</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int initialized</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 x86_mask</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 x86_capability[19]</code> ➡️ <code>__u32 x86_capability[20]</code>
</li>
<li>
<b>Field type changed. </b>
<code>int x86_cache_size</code> ➡️ <code>unsigned int x86_cache_size</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u8 x86_cache_bits</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 cpu_die_id</code>
</li>
<li>
<b>Field added. </b>
<code>u16 logical_die_id</code>
</li>
</ul>
</details>
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
<code>__u32 vmx_capability[3]</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int x86_capability_alignment</code>
</li>
<li>
<b>Field added. </b>
<code>int x86_cache_mbm_width_offset</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__u32 x86_capability[20]</code> ➡️ <code>__u32 x86_capability[21]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool smt_active</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 ppin</code>
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
<code>__u32 vmx_capability[3]</code> ➡️ <code>__u32 vmx_capability[5]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__u32 x86_capability[21]</code> ➡️ <code>__u32 x86_capability[23]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct cpuinfo_topology topo</code>
</li>
<li>
<b>Field removed. </b>
<code>__u8 cu_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 apicid</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 initial_apicid</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 phys_proc_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 logical_proc_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 cpu_core_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 cpu_die_id</code>
</li>
<li>
<b>Field removed. </b>
<code>u16 logical_die_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>__u32 x86_capability[23]</code> ➡️ <code>__u32 x86_capability[24]</code>
</li>
</ul>
</details>
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
