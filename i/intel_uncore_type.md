# Struct: <code>intel_uncore_type</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int mmio_map_size;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    const struct attribute_group **attr_update;
    struct pmu *pmu;
    u64 *topology;
    int (*set_mapping)(struct intel_uncore_type *);
    void (*cleanup_mapping)(struct intel_uncore_type *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    int type_id;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    u64 *box_ctls;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int mmio_map_size;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    unsigned int *pci_offsets;
    unsigned int *mmio_offsets;
    unsigned int *box_ids;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    const struct attribute_group **attr_update;
    struct pmu *pmu;
    struct intel_uncore_topology *topology;
    int (*set_mapping)(struct intel_uncore_type *);
    void (*cleanup_mapping)(struct intel_uncore_type *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    int type_id;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    u64 *box_ctls;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int mmio_map_size;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    unsigned int *pci_offsets;
    unsigned int *mmio_offsets;
    unsigned int *box_ids;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    const struct attribute_group **attr_update;
    struct pmu *pmu;
    struct intel_uncore_topology *topology;
    int (*get_topology)(struct intel_uncore_type *);
    int (*set_mapping)(struct intel_uncore_type *);
    void (*cleanup_mapping)(struct intel_uncore_type *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    int type_id;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    u64 *box_ctls;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int mmio_map_size;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    unsigned int *pci_offsets;
    unsigned int *mmio_offsets;
    unsigned int *box_ids;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    const struct attribute_group **attr_update;
    struct pmu *pmu;
    struct intel_uncore_topology *topology;
    int (*get_topology)(struct intel_uncore_type *);
    int (*set_mapping)(struct intel_uncore_type *);
    void (*cleanup_mapping)(struct intel_uncore_type *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    int type_id;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    u64 *box_ctls;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int mmio_map_size;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    unsigned int *pci_offsets;
    unsigned int *mmio_offsets;
    unsigned int *box_ids;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    const struct attribute_group **attr_update;
    struct pmu *pmu;
    struct intel_uncore_topology **topology;
    int (*get_topology)(struct intel_uncore_type *);
    void (*set_mapping)(struct intel_uncore_type *);
    void (*cleanup_mapping)(struct intel_uncore_type *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    int type_id;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    u64 *box_ctls;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int mmio_map_size;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    unsigned int *pci_offsets;
    unsigned int *mmio_offsets;
    unsigned int *box_ids;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    const struct attribute_group **attr_update;
    struct pmu *pmu;
    struct intel_uncore_topology **topology;
    int (*get_topology)(struct intel_uncore_type *);
    void (*set_mapping)(struct intel_uncore_type *);
    void (*cleanup_mapping)(struct intel_uncore_type *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    int type_id;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    u64 *box_ctls;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int mmio_map_size;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    u64 *msr_offsets;
    u64 *pci_offsets;
    u64 *mmio_offsets;
    unsigned int *box_ids;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    const struct attribute_group **attr_update;
    struct pmu *pmu;
    struct intel_uncore_topology **topology;
    int (*get_topology)(struct intel_uncore_type *);
    void (*set_mapping)(struct intel_uncore_type *);
    void (*cleanup_mapping)(struct intel_uncore_type *);
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
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct intel_uncore_type {
    const char *name;
    int num_counters;
    int num_boxes;
    int perf_ctr_bits;
    int fixed_ctr_bits;
    int num_freerunning_types;
    unsigned int perf_ctr;
    unsigned int event_ctl;
    unsigned int event_mask;
    unsigned int event_mask_ext;
    unsigned int fixed_ctr;
    unsigned int fixed_ctl;
    unsigned int box_ctl;
    unsigned int msr_offset;
    unsigned int mmio_offset;
    unsigned int num_shared_regs;
    unsigned int single_fixed;
    unsigned int pair_ctr_ctl;
    unsigned int *msr_offsets;
    struct event_constraint unconstrainted;
    struct event_constraint *constraints;
    struct intel_uncore_pmu *pmus;
    struct intel_uncore_ops *ops;
    struct uncore_event_desc *event_descs;
    struct freerunning_counters *freerunning;
    const struct attribute_group * attr_groups[4];
    struct pmu *pmu;
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
<code>unsigned int event_mask_ext</code>
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int num_freerunning_types</code>
</li>
<li>
<b>Field added. </b>
<code>struct freerunning_counters *freerunning</code>
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
<code>unsigned int mmio_offset</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>unsigned int mmio_map_size</code>
</li>
<li>
<b>Field added. </b>
<code>const struct attribute_group **attr_update</code>
</li>
<li>
<b>Field added. </b>
<code>u64 *topology</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_mapping)(struct intel_uncore_type *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*cleanup_mapping)(struct intel_uncore_type *)</code>
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
<code>int type_id</code>
</li>
<li>
<b>Field added. </b>
<code>u64 *box_ctls</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int *pci_offsets</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int *mmio_offsets</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int *box_ids</code>
</li>
<li>
<b>Field type changed. </b>
<code>u64 *topology</code> ➡️ <code>struct intel_uncore_topology *topology</code>
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
<code>int (*get_topology)(struct intel_uncore_type *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct intel_uncore_topology *topology</code> ➡️ <code>struct intel_uncore_topology **topology</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_mapping)(struct intel_uncore_type *)</code> ➡️ <code>void (*set_mapping)(struct intel_uncore_type *)</code>
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
<b>Field type changed. </b>
<code>unsigned int *msr_offsets</code> ➡️ <code>u64 *msr_offsets</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int *pci_offsets</code> ➡️ <code>u64 *pci_offsets</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int *mmio_offsets</code> ➡️ <code>u64 *mmio_offsets</code>
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
