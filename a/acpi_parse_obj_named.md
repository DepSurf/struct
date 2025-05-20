# Struct: <code>acpi_parse_obj_named</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u8 *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u8 *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u8 *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
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
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    char *path;
    u8 *data;
    u32 length;
    u32 name;
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
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_parse_obj_named {
    union acpi_parse_object *parent;
    u8 descriptor_type;
    u8 flags;
    u16 aml_opcode;
    u8 *aml;
    union acpi_parse_object *next;
    struct acpi_namespace_node *node;
    union acpi_parse_value value;
    u8 arg_list_length;
    u16 disasm_flags;
    u8 disasm_opcode;
    char *operator_symbol;
    char aml_op_name[16];
    char *path;
    u8 *data;
    u32 length;
    u32 name;
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
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 *path</code> ➡️ <code>char *path</code>
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
<code>u16 disasm_flags</code>
</li>
<li>
<b>Field added. </b>
<code>u8 disasm_opcode</code>
</li>
<li>
<b>Field added. </b>
<code>char *operator_symbol</code>
</li>
<li>
<b>Field added. </b>
<code>char aml_op_name[16]</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>amd64</code> and <code>arm64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u16 disasm_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 disasm_opcode</code>
</li>
<li>
<b>Field removed. </b>
<code>char *operator_symbol</code>
</li>
<li>
<b>Field removed. </b>
<code>char aml_op_name[16]</code>
</li>
</ul>
</details>
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>aws</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u16 disasm_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 disasm_opcode</code>
</li>
<li>
<b>Field removed. </b>
<code>char *operator_symbol</code>
</li>
<li>
<b>Field removed. </b>
<code>char aml_op_name[16]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>generic</code> and <code>azure</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u16 disasm_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>u8 disasm_opcode</code>
</li>
<li>
<b>Field removed. </b>
<code>char *operator_symbol</code>
</li>
<li>
<b>Field removed. </b>
<code>char aml_op_name[16]</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
