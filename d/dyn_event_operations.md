# Struct: <code>dyn_event_operations</code>

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
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(const char *);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(const char *);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(const char *);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(const char *);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(const char *);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(const char *);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
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
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
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
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dyn_event_operations {
    struct list_head list;
    int (*create)(int, const char **);
    int (*show)(struct seq_file *, struct dyn_event *);
    bool (*is_busy)(struct dyn_event *);
    int (*free)(struct dyn_event *);
    bool (*match)(const char *, const char *, int, const char **, struct dyn_event *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>bool (*match)(const char *, const char *, struct dyn_event *)</code> ➡️ <code>bool (*match)(const char *, const char *, int, const char **, struct dyn_event *)</code>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*create)(int, const char **)</code> ➡️ <code>int (*create)(const char *)</code>
</li>
</ul>
</details>
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
