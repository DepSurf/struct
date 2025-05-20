# Struct: <code>vmap_area</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct list_head purge_list;
    struct vm_struct *vm;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct llist_node purge_list;
    struct vm_struct *vm;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct llist_node purge_list;
    struct vm_struct *vm;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct llist_node purge_list;
    struct vm_struct *vm;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct llist_node purge_list;
    struct vm_struct *vm;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct llist_node purge_list;
    struct vm_struct *vm;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct llist_node purge_list;
    struct vm_struct *vm;
    struct callback_head callback_head;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    long unsigned int subtree_max_size;
    long unsigned int flags;
    struct rb_node rb_node;
    struct list_head list;
    struct llist_node purge_list;
    struct vm_struct *vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    long unsigned int flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    long unsigned int flags;
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
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
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
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct vmap_area {
    long unsigned int va_start;
    long unsigned int va_end;
    struct rb_node rb_node;
    struct list_head list;
    long unsigned int subtree_max_size;
    struct vm_struct *vm;
    struct llist_node purge_list;
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
<code>struct list_head purge_list</code> ➡️ <code>struct llist_node purge_list</code>
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int subtree_max_size</code>
</li>
<li>
<b>Field removed. </b>
<code>struct callback_head callback_head</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>long unsigned int flags</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct llist_node purge_list</code>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>long unsigned int flags</code>
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
