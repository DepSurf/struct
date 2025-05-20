# Struct: <code>paravirt_patch_template</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops pv_init_ops;
    struct pv_time_ops pv_time_ops;
    struct pv_cpu_ops pv_cpu_ops;
    struct pv_irq_ops pv_irq_ops;
    struct pv_apic_ops pv_apic_ops;
    struct pv_mmu_ops pv_mmu_ops;
    struct pv_lock_ops pv_lock_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops pv_init_ops;
    struct pv_time_ops pv_time_ops;
    struct pv_cpu_ops pv_cpu_ops;
    struct pv_irq_ops pv_irq_ops;
    struct pv_mmu_ops pv_mmu_ops;
    struct pv_lock_ops pv_lock_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops pv_init_ops;
    struct pv_time_ops pv_time_ops;
    struct pv_cpu_ops pv_cpu_ops;
    struct pv_irq_ops pv_irq_ops;
    struct pv_mmu_ops pv_mmu_ops;
    struct pv_lock_ops pv_lock_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops pv_init_ops;
    struct pv_time_ops pv_time_ops;
    struct pv_cpu_ops pv_cpu_ops;
    struct pv_irq_ops pv_irq_ops;
    struct pv_mmu_ops pv_mmu_ops;
    struct pv_lock_ops pv_lock_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops pv_init_ops;
    struct pv_time_ops pv_time_ops;
    struct pv_cpu_ops pv_cpu_ops;
    struct pv_irq_ops pv_irq_ops;
    struct pv_mmu_ops pv_mmu_ops;
    struct pv_lock_ops pv_lock_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops pv_init_ops;
    struct pv_time_ops pv_time_ops;
    struct pv_cpu_ops pv_cpu_ops;
    struct pv_irq_ops pv_irq_ops;
    struct pv_mmu_ops pv_mmu_ops;
    struct pv_lock_ops pv_lock_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
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
struct paravirt_patch_template {
    struct pv_time_ops time;
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
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct paravirt_patch_template {
    struct pv_init_ops init;
    struct pv_time_ops time;
    struct pv_cpu_ops cpu;
    struct pv_irq_ops irq;
    struct pv_mmu_ops mmu;
    struct pv_lock_ops lock;
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
<code>struct pv_apic_ops pv_apic_ops</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct pv_init_ops init</code>
</li>
<li>
<b>Field added. </b>
<code>struct pv_time_ops time</code>
</li>
<li>
<b>Field added. </b>
<code>struct pv_cpu_ops cpu</code>
</li>
<li>
<b>Field added. </b>
<code>struct pv_irq_ops irq</code>
</li>
<li>
<b>Field added. </b>
<code>struct pv_mmu_ops mmu</code>
</li>
<li>
<b>Field added. </b>
<code>struct pv_lock_ops lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_init_ops pv_init_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_time_ops pv_time_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_cpu_ops pv_cpu_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_irq_ops pv_irq_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_mmu_ops pv_mmu_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_lock_ops pv_lock_ops</code>
</li>
</ul>
</details>
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
<b>Field removed. </b>
<code>struct pv_init_ops init</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_time_ops time</code>
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
<b>Field removed. </b>
<code>struct pv_init_ops init</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_cpu_ops cpu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_irq_ops irq</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_mmu_ops mmu</code>
</li>
<li>
<b>Field removed. </b>
<code>struct pv_lock_ops lock</code>
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
