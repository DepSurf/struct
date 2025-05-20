# Struct: <code>kvm_pmc</code>

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
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kvm_pmc {
    enum pmc_type type;
    u8 idx;
    u64 counter;
    u64 eventsel;
    struct perf_event *perf_event;
    struct kvm_vcpu *vcpu;
    u64 current_config;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kvm_pmc {
    enum pmc_type type;
    u8 idx;
    u64 counter;
    u64 eventsel;
    struct perf_event *perf_event;
    struct kvm_vcpu *vcpu;
    u64 current_config;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kvm_pmc {
    enum pmc_type type;
    u8 idx;
    u64 counter;
    u64 eventsel;
    struct perf_event *perf_event;
    struct kvm_vcpu *vcpu;
    u64 current_config;
    bool is_paused;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kvm_pmc {
    enum pmc_type type;
    u8 idx;
    u64 counter;
    u64 eventsel;
    struct perf_event *perf_event;
    struct kvm_vcpu *vcpu;
    u64 current_config;
    bool is_paused;
    bool intr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kvm_pmc {
    enum pmc_type type;
    u8 idx;
    bool is_paused;
    bool intr;
    u64 counter;
    u64 prev_counter;
    u64 eventsel;
    struct perf_event *perf_event;
    struct kvm_vcpu *vcpu;
    u64 current_config;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kvm_pmc {
    enum pmc_type type;
    u8 idx;
    bool is_paused;
    bool intr;
    u64 counter;
    u64 prev_counter;
    u64 eventsel;
    struct perf_event *perf_event;
    struct kvm_vcpu *vcpu;
    u64 current_config;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kvm_pmc {
    enum pmc_type type;
    u8 idx;
    bool is_paused;
    bool intr;
    u64 counter;
    u64 emulated_counter;
    u64 eventsel;
    struct perf_event *perf_event;
    struct kvm_vcpu *vcpu;
    u64 current_config;
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
struct kvm_pmc {
    u8 idx;
    struct perf_event *perf_event;
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool is_paused</code>
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
<code>bool intr</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 prev_counter</code>
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
<code>u64 emulated_counter</code>
</li>
<li>
<b>Field removed. </b>
<code>u64 prev_counter</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Arch</b>
<ul>
</ul>
