# Struct: <code>software_node</code>

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
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct software_node {
    int id;
    struct kobject kobj;
    struct fwnode_handle fwnode;
    struct ida child_ids;
    struct list_head entry;
    struct list_head children;
    struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
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
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
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
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct software_node {
    const char *name;
    const struct software_node *parent;
    const struct property_entry *properties;
    const struct software_node_reference *references;
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
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const char *name</code>
</li>
<li>
<b>Field added. </b>
<code>const struct software_node_reference *references</code>
</li>
<li>
<b>Field removed. </b>
<code>int id</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kobject kobj</code>
</li>
<li>
<b>Field removed. </b>
<code>struct fwnode_handle fwnode</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ida child_ids</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head entry</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head children</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct software_node *parent</code> ➡️ <code>const struct software_node *parent</code>
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
<b>Field removed. </b>
<code>const struct software_node_reference *references</code>
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
