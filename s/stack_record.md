# Struct: <code>stack_record</code>

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
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct stack_record {
    struct stack_record *next;
    u32 hash;
    u32 size;
    union handle_parts handle;
    long unsigned int entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct stack_record {
    struct stack_record *next;
    u32 hash;
    u32 size;
    union handle_parts handle;
    long unsigned int entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct stack_record {
    struct stack_record *next;
    u32 hash;
    u32 size;
    union handle_parts handle;
    long unsigned int entries[0];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct stack_record {
    struct list_head hash_list;
    u32 hash;
    u32 size;
    union handle_parts handle;
    refcount_t count;
    long unsigned int entries[64];
    struct list_head free_list;
    long unsigned int rcu_state;
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
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.19</code> and <code>6.2</code> ✅
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct list_head hash_list</code>
</li>
<li>
<b>Field added. </b>
<code>refcount_t count</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head free_list</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int rcu_state</code>
</li>
<li>
<b>Field removed. </b>
<code>struct stack_record *next</code>
</li>
<li>
<b>Field type changed. </b>
<code>long unsigned int entries[0]</code> ➡️ <code>long unsigned int entries[64]</code>
</li>
</ul>
</details>
</li>
</ul>
