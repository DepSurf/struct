# Struct: <code>ima_rule_entry</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    u8 fsuuid[16];
    kuid_t uid;
    kuid_t fowner;
    struct (anon) lsm[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    u8 fsuuid[16];
    kuid_t uid;
    kuid_t fowner;
    int pcr;
    struct (anon) lsm[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    u8 fsuuid[16];
    kuid_t uid;
    kuid_t fowner;
    int pcr;
    struct (anon) lsm[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    char *keyrings;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_rule_opt_list *keyrings;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_rule_opt_list *keyrings;
    struct ima_rule_opt_list *label;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    unsigned int allowed_algos;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_rule_opt_list *keyrings;
    struct ima_rule_opt_list *label;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kgid_t gid;
    kuid_t fowner;
    kgid_t fgroup;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*gid_op)(kgid_t, kgid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    bool (*fgroup_op)(kgid_t, kgid_t);
    int pcr;
    unsigned int allowed_algos;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_rule_opt_list *keyrings;
    struct ima_rule_opt_list *label;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kgid_t gid;
    kuid_t fowner;
    kgid_t fgroup;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*gid_op)(kgid_t, kgid_t);
    bool (*fowner_op)(vfsuid_t, kuid_t);
    bool (*fgroup_op)(vfsgid_t, kgid_t);
    int pcr;
    unsigned int allowed_algos;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_rule_opt_list *keyrings;
    struct ima_rule_opt_list *label;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kgid_t gid;
    kuid_t fowner;
    kgid_t fgroup;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*gid_op)(kgid_t, kgid_t);
    bool (*fowner_op)(vfsuid_t, kuid_t);
    bool (*fgroup_op)(vfsgid_t, kgid_t);
    int pcr;
    unsigned int allowed_algos;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_rule_opt_list *keyrings;
    struct ima_rule_opt_list *label;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kgid_t gid;
    kuid_t fowner;
    kgid_t fgroup;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*gid_op)(kgid_t, kgid_t);
    bool (*fowner_op)(vfsuid_t, kuid_t);
    bool (*fgroup_op)(vfsgid_t, kgid_t);
    int pcr;
    unsigned int allowed_algos;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_rule_opt_list *keyrings;
    struct ima_rule_opt_list *label;
    struct ima_template_desc *template;
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
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
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
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ima_rule_entry {
    struct list_head list;
    int action;
    unsigned int flags;
    enum ima_hooks func;
    int mask;
    long unsigned int fsmagic;
    uuid_t fsuuid;
    kuid_t uid;
    kuid_t fowner;
    bool (*uid_op)(kuid_t, kuid_t);
    bool (*fowner_op)(kuid_t, kuid_t);
    int pcr;
    struct (anon) lsm[6];
    char *fsname;
    struct ima_template_desc *template;
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
<code>int pcr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*uid_op)(kuid_t, kuid_t)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*fowner_op)(kuid_t, kuid_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>u8 fsuuid[16]</code> ➡️ <code>uuid_t fsuuid</code>
</li>
</ul>
</details>
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
<code>char *fsname</code>
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
<code>struct ima_template_desc *template</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>char *keyrings</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>char *keyrings</code> ➡️ <code>struct ima_rule_opt_list *keyrings</code>
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
<code>struct ima_rule_opt_list *label</code>
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
<code>unsigned int allowed_algos</code>
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
<code>kgid_t gid</code>
</li>
<li>
<b>Field added. </b>
<code>kgid_t fgroup</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*gid_op)(kgid_t, kgid_t)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*fgroup_op)(kgid_t, kgid_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>bool (*fowner_op)(kuid_t, kuid_t)</code> ➡️ <code>bool (*fowner_op)(vfsuid_t, kuid_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*fgroup_op)(kgid_t, kgid_t)</code> ➡️ <code>bool (*fgroup_op)(vfsgid_t, kgid_t)</code>
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
