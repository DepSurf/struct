# Struct: <code>fs_context</code>

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
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    const char *subtype;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct p_log log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
    bool oldapi;
    bool exclusive;
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
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
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
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct fs_context {
    const struct fs_context_operations *ops;
    struct mutex uapi_mutex;
    struct file_system_type *fs_type;
    void *fs_private;
    void *sget_key;
    struct dentry *root;
    struct user_namespace *user_ns;
    struct net *net_ns;
    const struct cred *cred;
    struct fc_log *log;
    const char *source;
    void *security;
    void *s_fs_info;
    unsigned int sb_flags;
    unsigned int sb_flags_mask;
    unsigned int s_iflags;
    unsigned int lsm_flags;
    enum fs_context_purpose purpose;
    enum fs_context_phase phase;
    bool need_free;
    bool global;
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
<code>void *sget_key</code>
</li>
<li>
<b>Field removed. </b>
<code>const char *subtype</code>
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
<code>bool oldapi</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct fc_log *log</code> ➡️ <code>struct p_log log</code>
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
<code>unsigned int lsm_flags</code>
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
<code>bool exclusive</code>
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
