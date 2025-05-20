# Struct: <code>unwind_state</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    struct pt_regs *regs;
    long unsigned int ip;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    struct llist_node *kr_cur;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    struct llist_node *kr_cur;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    struct llist_node *kr_cur;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    struct llist_node *kr_cur;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct unwind_state {
    struct stack_info stack_info;
    long unsigned int stack_mask;
    struct task_struct *task;
    int graph_idx;
    bool error;
    bool got_irq;
    long unsigned int *bp;
    long unsigned int *orig_sp;
    long unsigned int ip;
    long unsigned int *next_bp;
    struct pt_regs *regs;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool error</code>
</li>
<li>
<b>Field added. </b>
<code>bool got_irq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int ip</code>
</li>
</ul>
</details>
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
<code>long unsigned int *next_bp</code>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct llist_node *kr_cur</code>
</li>
</ul>
</details>
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
