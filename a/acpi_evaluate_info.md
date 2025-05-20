# Struct: <code>acpi_evaluate_info</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u8 pass_number;
    u8 return_object_type;
    u8 node_flags;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
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
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_evaluate_info {
    struct acpi_namespace_node *prefix_node;
    const char *relative_pathname;
    union acpi_operand_object **parameters;
    struct acpi_namespace_node *node;
    union acpi_operand_object *obj_desc;
    char *full_pathname;
    const union acpi_predefined_info *predefined;
    union acpi_operand_object *return_object;
    union acpi_operand_object *parent_package;
    u32 return_flags;
    u32 return_btype;
    u16 param_count;
    u16 node_flags;
    u8 pass_number;
    u8 return_object_type;
    u8 flags;
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
<b>Field type changed. </b>
<code>char *relative_pathname</code> ➡️ <code>const char *relative_pathname</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
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
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 node_flags</code> ➡️ <code>u16 node_flags</code>
</li>
</ul>
</details>
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
