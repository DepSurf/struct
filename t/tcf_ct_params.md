# Struct: <code>tcf_ct_params</code>

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
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
    struct tcf_ct_flow_table *ct_ft;
    struct nf_flowtable *nf_ft;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
    struct tcf_ct_flow_table *ct_ft;
    struct nf_flowtable *nf_ft;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
    struct tcf_ct_flow_table *ct_ft;
    struct nf_flowtable *nf_ft;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
    struct tcf_ct_flow_table *ct_ft;
    struct nf_flowtable *nf_ft;
};
```
</details>
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
</li>
</ul>
<b>Arch</b>
<ul>
<li>
<details>
<summary>In <code>arm64</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tcf_ct_params {
    struct nf_conn *tmpl;
    u16 zone;
    u32 mark;
    u32 mark_mask;
    u32 labels[4];
    u32 labels_mask[4];
    struct nf_nat_range2 range;
    bool ipv4_range;
    u16 ct_action;
    struct callback_head rcu;
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct tcf_ct_flow_table *ct_ft</code>
</li>
<li>
<b>Field added. </b>
<code>struct nf_flowtable *nf_ft</code>
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
</ul>
<b>Arch</b>
<ul>
<li>
No changes between <code>amd64</code> and <code>arm64</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>armhf</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
No changes between <code>amd64</code> and <code>riscv64</code> ✅
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
