# Struct: <code>class</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    struct class_attribute *class_attrs;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    struct class_attribute *class_attrs;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    struct class_attribute *class_attrs;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*suspend)(struct device *, pm_message_t);
    int (*resume)(struct device *);
    int (*shutdown)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(const struct device *, struct kobj_uevent_env *);
    char * (*devnode)(const struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(const struct device *);
    void (*get_ownership)(const struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct class {
    const char *name;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    int (*dev_uevent)(const struct device *, struct kobj_uevent_env *);
    char * (*devnode)(const struct device *, umode_t *);
    void (*class_release)(const struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(const struct device *);
    void (*get_ownership)(const struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct class {
    const char *name;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    int (*dev_uevent)(const struct device *, struct kobj_uevent_env *);
    char * (*devnode)(const struct device *, umode_t *);
    void (*class_release)(const struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(const struct device *);
    void (*get_ownership)(const struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
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
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
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
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct class {
    const char *name;
    struct module *owner;
    const struct attribute_group **class_groups;
    const struct attribute_group **dev_groups;
    struct kobject *dev_kobj;
    int (*dev_uevent)(struct device *, struct kobj_uevent_env *);
    char * (*devnode)(struct device *, umode_t *);
    void (*class_release)(struct class *);
    void (*dev_release)(struct device *);
    int (*shutdown_pre)(struct device *);
    const struct kobj_ns_type_operations *ns_type;
    const void * (*namespace)(struct device *);
    void (*get_ownership)(struct device *, kuid_t *, kgid_t *);
    const struct dev_pm_ops *pm;
    struct subsys_private *p;
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
<code>const struct attribute_group **class_groups</code>
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
<code>int (*shutdown)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct class_attribute *class_attrs</code>
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
<code>int (*shutdown_pre)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*suspend)(struct device *, pm_message_t)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*resume)(struct device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*shutdown)(struct device *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*get_ownership)(struct device *, kuid_t *, kgid_t *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*dev_uevent)(struct device *, struct kobj_uevent_env *)</code> ➡️ <code>int (*dev_uevent)(const struct device *, struct kobj_uevent_env *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>char * (*devnode)(struct device *, umode_t *)</code> ➡️ <code>char * (*devnode)(const struct device *, umode_t *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>const void * (*namespace)(struct device *)</code> ➡️ <code>const void * (*namespace)(const struct device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*get_ownership)(struct device *, kuid_t *, kgid_t *)</code> ➡️ <code>void (*get_ownership)(const struct device *, kuid_t *, kgid_t *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kobject *dev_kobj</code>
</li>
<li>
<b>Field removed. </b>
<code>struct subsys_private *p</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*class_release)(struct class *)</code> ➡️ <code>void (*class_release)(const struct class *)</code>
</li>
</ul>
</details>
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
