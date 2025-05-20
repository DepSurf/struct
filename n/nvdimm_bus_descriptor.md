# Struct: <code>nvdimm_bus_descriptor</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int dsm_mask;
    char *provider_name;
    ndctl_fn ndctl;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
    const struct nvdimm_bus_fw_ops *fw_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
    const struct nvdimm_bus_fw_ops *fw_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
    const struct nvdimm_bus_fw_ops *fw_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
    const struct nvdimm_bus_fw_ops *fw_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
    const struct nvdimm_bus_fw_ops *fw_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
    const struct nvdimm_bus_fw_ops *fw_ops;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int cmd_mask;
    long unsigned int dimm_family_mask;
    long unsigned int bus_family_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
    const struct nvdimm_bus_fw_ops *fw_ops;
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
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
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
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct nvdimm_bus_descriptor {
    const struct attribute_group **attr_groups;
    long unsigned int bus_dsm_mask;
    long unsigned int cmd_mask;
    struct module *module;
    char *provider_name;
    struct device_node *of_node;
    ndctl_fn ndctl;
    int (*flush_probe)(struct nvdimm_bus_descriptor *);
    int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *);
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
<code>long unsigned int cmd_mask</code>
</li>
<li>
<b>Field added. </b>
<code>struct module *module</code>
</li>
<li>
<b>Field added. </b>
<code>int (*flush_probe)(struct nvdimm_bus_descriptor *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int dsm_mask</code>
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
<code>long unsigned int bus_dsm_mask</code>
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
<code>struct device_node *of_node</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int)</code> ➡️ <code>int (*clear_to_send)(struct nvdimm_bus_descriptor *, struct nvdimm *, unsigned int, void *)</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int dimm_family_mask</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int bus_family_mask</code>
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
<code>const struct nvdimm_bus_fw_ops *fw_ops</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int bus_dsm_mask</code>
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
