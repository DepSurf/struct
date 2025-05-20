# Struct: <code>kfree_rcu_cpu_work</code>

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
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct kfree_rcu_bulk_data *bhead_free;
    struct kfree_rcu_cpu *krcp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct kvfree_rcu_bulk_data * bkvhead_free[2];
    struct kfree_rcu_cpu *krcp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct kvfree_rcu_bulk_data * bkvhead_free[2];
    struct kfree_rcu_cpu *krcp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct kvfree_rcu_bulk_data * bkvhead_free[2];
    struct kfree_rcu_cpu *krcp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct kvfree_rcu_bulk_data * bkvhead_free[2];
    struct kfree_rcu_cpu *krcp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct kvfree_rcu_bulk_data * bkvhead_free[2];
    struct kfree_rcu_cpu *krcp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct rcu_gp_oldstate head_free_gp_snap;
    struct list_head bulk_head_free[2];
    struct kfree_rcu_cpu *krcp;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kfree_rcu_cpu_work {
    struct rcu_work rcu_work;
    struct callback_head *head_free;
    struct rcu_gp_oldstate head_free_gp_snap;
    struct list_head bulk_head_free[2];
    struct kfree_rcu_cpu *krcp;
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
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct kvfree_rcu_bulk_data * bkvhead_free[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kfree_rcu_bulk_data *bhead_free</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct rcu_gp_oldstate head_free_gp_snap</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head bulk_head_free[2]</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kvfree_rcu_bulk_data * bkvhead_free[2]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
