# Struct: <code>ctrl_dump_policy_ctx</code>

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
struct ctrl_dump_policy_ctx {
    struct netlink_policy_dump_state *state;
    const struct genl_family *rt;
    unsigned int opidx;
    u32 op;
    u16 fam_id;
    u8 policies;
    u8 single_op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ctrl_dump_policy_ctx {
    struct netlink_policy_dump_state *state;
    const struct genl_family *rt;
    unsigned int opidx;
    u32 op;
    u16 fam_id;
    u8 policies;
    u8 single_op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ctrl_dump_policy_ctx {
    struct netlink_policy_dump_state *state;
    const struct genl_family *rt;
    unsigned int opidx;
    u32 op;
    u16 fam_id;
    u8 policies;
    u8 single_op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ctrl_dump_policy_ctx {
    struct netlink_policy_dump_state *state;
    const struct genl_family *rt;
    unsigned int opidx;
    u32 op;
    u16 fam_id;
    u8 policies;
    u8 single_op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ctrl_dump_policy_ctx {
    struct netlink_policy_dump_state *state;
    const struct genl_family *rt;
    struct genl_op_iter *op_iter;
    u32 op;
    u16 fam_id;
    u8 dump_map;
    u8 single_op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ctrl_dump_policy_ctx {
    struct netlink_policy_dump_state *state;
    const struct genl_family *rt;
    struct genl_op_iter *op_iter;
    u32 op;
    u16 fam_id;
    u8 dump_map;
    u8 single_op;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ctrl_dump_policy_ctx {
    struct netlink_policy_dump_state *state;
    const struct genl_family *rt;
    struct genl_op_iter *op_iter;
    u32 op;
    u16 fam_id;
    u8 dump_map;
    u8 single_op;
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
No changes between <code>5.11</code> and <code>5.13</code> ✅
</li>
<li>
No changes between <code>5.13</code> and <code>5.15</code> ✅
</li>
<li>
No changes between <code>5.15</code> and <code>5.19</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct genl_op_iter *op_iter</code>
</li>
<li>
<b>Field added. </b>
<code>u8 dump_map</code>
</li>
<li>
<b>Field removed. </b>
<code>unsigned int opidx</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 policies</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
