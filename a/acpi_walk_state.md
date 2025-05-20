# Struct: <code>acpi_walk_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
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
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
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
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_walk_state {
    struct acpi_walk_state *next;
    u8 descriptor_type;
    u8 walk_type;
    u16 opcode;
    u8 next_op_info;
    u8 num_operands;
    u8 operand_index;
    acpi_owner_id owner_id;
    u8 last_predicate;
    u8 current_result;
    u8 return_used;
    u8 scope_depth;
    u8 pass_number;
    u8 namespace_override;
    u8 result_size;
    u8 result_count;
    u8 *aml;
    u32 arg_types;
    u32 method_breakpoint;
    u32 user_breakpoint;
    u32 parse_flags;
    struct acpi_parse_state parser_state;
    u32 prev_arg_types;
    u32 arg_count;
    u16 method_nesting_depth;
    u8 method_is_nested;
    struct acpi_namespace_node arguments[7];
    struct acpi_namespace_node local_variables[8];
    union acpi_operand_object * operands[9];
    union acpi_operand_object **params;
    u8 *aml_last_while;
    union acpi_operand_object **caller_return_desc;
    union acpi_generic_state *control_state;
    struct acpi_namespace_node *deferred_node;
    union acpi_operand_object *implicit_return_obj;
    struct acpi_namespace_node *method_call_node;
    union acpi_parse_object *method_call_op;
    union acpi_operand_object *method_desc;
    struct acpi_namespace_node *method_node;
    char *method_pathname;
    union acpi_parse_object *op;
    const struct acpi_opcode_info *op_info;
    union acpi_parse_object *origin;
    union acpi_operand_object *result_obj;
    union acpi_generic_state *results;
    union acpi_operand_object *return_desc;
    union acpi_generic_state *scope_info;
    union acpi_parse_object *prev_op;
    union acpi_parse_object *next_op;
    struct acpi_thread_state *thread;
    acpi_parse_downwards descending_callback;
    acpi_parse_upwards ascending_callback;
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
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
No changes between <code>4.15</code> and <code>4.18</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 method_nesting_depth</code>
</li>
<li>
<b>Field added. </b>
<code>u8 method_is_nested</code>
</li>
<li>
<b>Field added. </b>
<code>char *method_pathname</code>
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
