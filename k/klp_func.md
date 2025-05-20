# Struct: <code>klp_func</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    long unsigned int old_addr;
    struct kobject kobj;
    enum klp_state state;
    struct list_head stack_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    long unsigned int old_addr;
    struct kobject kobj;
    enum klp_state state;
    struct list_head stack_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    long unsigned int old_addr;
    struct kobject kobj;
    enum klp_state state;
    struct list_head stack_node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    bool immediate;
    long unsigned int old_addr;
    struct kobject kobj;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    bool immediate;
    long unsigned int old_addr;
    struct kobject kobj;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    long unsigned int old_addr;
    struct kobject kobj;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    long unsigned int old_addr;
    struct kobject kobj;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
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
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct klp_func {
    const char *old_name;
    void *new_func;
    long unsigned int old_sympos;
    void *old_func;
    struct kobject kobj;
    struct list_head node;
    struct list_head stack_node;
    long unsigned int old_size;
    long unsigned int new_size;
    bool nop;
    bool patched;
    bool transition;
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
<b>Field added. </b>
<code>bool immediate</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int old_size</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int new_size</code>
</li>
<li>
<b>Field added. </b>
<code>bool patched</code>
</li>
<li>
<b>Field added. </b>
<code>bool transition</code>
</li>
<li>
<b>Field removed. </b>
<code>enum klp_state state</code>
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
<b>Field removed. </b>
<code>bool immediate</code>
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
<code>void *old_func</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head node</code>
</li>
<li>
<b>Field added. </b>
<code>bool nop</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int old_addr</code>
</li>
</ul>
</details>
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
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
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
