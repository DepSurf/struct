# Struct: <code>quotactl_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
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
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
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
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct quotactl_ops {
    int (*quota_on)(struct super_block *, int, int, const struct path *);
    int (*quota_off)(struct super_block *, int);
    int (*quota_enable)(struct super_block *, unsigned int);
    int (*quota_disable)(struct super_block *, unsigned int);
    int (*quota_sync)(struct super_block *, int);
    int (*set_info)(struct super_block *, int, struct qc_info *);
    int (*get_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *);
    int (*set_dqblk)(struct super_block *, struct kqid, struct qc_dqblk *);
    int (*get_state)(struct super_block *, struct qc_state *);
    int (*rm_xquota)(struct super_block *, unsigned int);
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
<b>Field added. </b>
<code>int (*get_nextdqblk)(struct super_block *, struct kqid *, struct qc_dqblk *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*quota_on)(struct super_block *, int, int, struct path *)</code> ➡️ <code>int (*quota_on)(struct super_block *, int, int, const struct path *)</code>
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
