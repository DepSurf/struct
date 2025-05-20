# Struct: <code>kernfs_syscall_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*remount_fs)(struct kernfs_root *, int *, char *);
    int (*show_options)(struct seq_file *, struct dentry *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*remount_fs)(struct kernfs_root *, int *, char *);
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*remount_fs)(struct kernfs_root *, int *, char *);
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*remount_fs)(struct kernfs_root *, int *, char *);
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*remount_fs)(struct kernfs_root *, int *, char *);
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*remount_fs)(struct kernfs_root *, int *, char *);
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*remount_fs)(struct kernfs_root *, int *, char *);
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
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
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
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
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct kernfs_syscall_ops {
    int (*show_options)(struct seq_file *, struct kernfs_root *);
    int (*mkdir)(struct kernfs_node *, const char *, umode_t);
    int (*rmdir)(struct kernfs_node *);
    int (*rename)(struct kernfs_node *, struct kernfs_node *, const char *);
    int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *);
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
<code>int (*show_path)(struct seq_file *, struct kernfs_node *, struct kernfs_root *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*show_options)(struct seq_file *, struct dentry *, struct kernfs_root *)</code> ➡️ <code>int (*show_options)(struct seq_file *, struct kernfs_root *)</code>
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
<b>Field removed. </b>
<code>int (*remount_fs)(struct kernfs_root *, int *, char *)</code>
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
