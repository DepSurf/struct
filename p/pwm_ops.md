# Struct: <code>pwm_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
    void (*dbg_show)(struct pwm_chip *, struct seq_file *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
    int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*dbg_show)(struct pwm_chip *, struct seq_file *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
    int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*dbg_show)(struct pwm_chip *, struct seq_file *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
    int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*dbg_show)(struct pwm_chip *, struct seq_file *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
    int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*dbg_show)(struct pwm_chip *, struct seq_file *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
    int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*dbg_show)(struct pwm_chip *, struct seq_file *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
    int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*dbg_show)(struct pwm_chip *, struct seq_file *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    int (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    int (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    int (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
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
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
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
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct pwm_ops {
    int (*request)(struct pwm_chip *, struct pwm_device *);
    void (*free)(struct pwm_chip *, struct pwm_device *);
    int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int);
    int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *);
    void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *);
    struct module *owner;
    int (*config)(struct pwm_chip *, struct pwm_device *, int, int);
    int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity);
    int (*enable)(struct pwm_chip *, struct pwm_device *);
    void (*disable)(struct pwm_chip *, struct pwm_device *);
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
<code>int (*capture)(struct pwm_chip *, struct pwm_device *, struct pwm_capture *, long unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *)</code>
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
<code>void (*dbg_show)(struct pwm_chip *, struct seq_file *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*apply)(struct pwm_chip *, struct pwm_device *, struct pwm_state *)</code> ➡️ <code>int (*apply)(struct pwm_chip *, struct pwm_device *, const struct pwm_state *)</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*config)(struct pwm_chip *, struct pwm_device *, int, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_polarity)(struct pwm_chip *, struct pwm_device *, enum pwm_polarity)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*enable)(struct pwm_chip *, struct pwm_device *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*disable)(struct pwm_chip *, struct pwm_device *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *)</code> ➡️ <code>int (*get_state)(struct pwm_chip *, struct pwm_device *, struct pwm_state *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct module *owner</code>
</li>
</ul>
</details>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
