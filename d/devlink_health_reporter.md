# Struct: <code>devlink_health_reporter</code>

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
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_port *devlink_port;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_port *devlink_port;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_port *devlink_port;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_port *devlink_port;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_port *devlink_port;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_port *devlink_port;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_port *devlink_port;
    struct devlink_fmsg *dump_fmsg;
    u64 graceful_period;
    bool auto_recover;
    bool auto_dump;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
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
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
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
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct devlink_health_reporter {
    struct list_head list;
    void *priv;
    const struct devlink_health_reporter_ops *ops;
    struct devlink *devlink;
    struct devlink_fmsg *dump_fmsg;
    struct mutex dump_lock;
    u64 graceful_period;
    bool auto_recover;
    u8 health_state;
    u64 dump_ts;
    u64 dump_real_ts;
    u64 error_count;
    u64 recovery_count;
    u64 last_recovery_ts;
    refcount_t refcount;
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
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 dump_real_ts</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool auto_dump</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct devlink_port *devlink_port</code>
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
<b>Field removed. </b>
<code>refcount_t refcount</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct mutex dump_lock</code>
</li>
</ul>
</details>
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
