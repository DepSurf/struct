# Struct: <code>hypervisor_x86</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    void (*set_cpu_features)(struct cpuinfo_x86 *);
    void (*init_platform)();
    bool (*x2apic_available)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    void (*set_cpu_features)(struct cpuinfo_x86 *);
    void (*init_platform)();
    bool (*x2apic_available)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    void (*set_cpu_features)(struct cpuinfo_x86 *);
    void (*init_platform)();
    bool (*x2apic_available)();
    void (*pin_vcpu)(int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    void (*init_platform)();
    bool (*x2apic_available)();
    void (*pin_vcpu)(int);
    void (*init_mem_mapping)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
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
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct hypervisor_x86 {
    const char *name;
    uint32_t (*detect)();
    enum x86_hypervisor_type type;
    struct x86_hyper_init init;
    struct x86_hyper_runtime runtime;
    bool ignore_nopv;
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
<code>void (*pin_vcpu)(int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*init_mem_mapping)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*set_cpu_features)(struct cpuinfo_x86 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum x86_hypervisor_type type</code>
</li>
<li>
<b>Field added. </b>
<code>struct x86_hyper_init init</code>
</li>
<li>
<b>Field added. </b>
<code>struct x86_hyper_runtime runtime</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*init_platform)()</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*x2apic_available)()</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*pin_vcpu)(int)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*init_mem_mapping)()</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<code>bool ignore_nopv</code>
</li>
</ul>
</details>
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
