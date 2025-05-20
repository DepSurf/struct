# Struct: <code>acpi_db_method_info</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[4];
    char * arguments[4];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_db_method_info {
    acpi_handle method;
    acpi_handle main_thread_gate;
    acpi_handle thread_complete_gate;
    acpi_handle info_gate;
    u64 *threads;
    u32 num_threads;
    u32 num_created;
    u32 num_completed;
    char *name;
    u32 flags;
    u32 num_loops;
    char pathname[512];
    char **args;
    acpi_object_type *types;
    char init_args;
    acpi_object_type arg_types[7];
    char * arguments[7];
    char num_threads_str[11];
    char id_of_thread_str[11];
    char index_of_thread_str[11];
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>acpi_object_type arg_types[4]</code> ➡️ <code>acpi_object_type arg_types[7]</code>
</li>
<li>
<b>Field type changed. </b>
<code>char * arguments[4]</code> ➡️ <code>char * arguments[7]</code>
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
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
