# Struct: <code>tpm_class_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tpm_class_ops {
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    bool (*update_timeouts)(struct tpm_chip *, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    bool (*update_timeouts)(struct tpm_chip *, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    bool (*update_timeouts)(struct tpm_chip *, long unsigned int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    bool (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*request_locality)(struct tpm_chip *, int);
    void (*relinquish_locality)(struct tpm_chip *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    bool (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*request_locality)(struct tpm_chip *, int);
    void (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    bool (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    bool (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    void (*update_durations)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
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
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
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
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tpm_class_ops {
    unsigned int flags;
    const u8 req_complete_mask;
    const u8 req_complete_val;
    bool (*req_canceled)(struct tpm_chip *, u8);
    int (*recv)(struct tpm_chip *, u8 *, size_t);
    int (*send)(struct tpm_chip *, u8 *, size_t);
    void (*cancel)(struct tpm_chip *);
    u8 (*status)(struct tpm_chip *);
    void (*update_timeouts)(struct tpm_chip *, long unsigned int *);
    int (*go_idle)(struct tpm_chip *);
    int (*cmd_ready)(struct tpm_chip *);
    int (*request_locality)(struct tpm_chip *, int);
    int (*relinquish_locality)(struct tpm_chip *, int);
    void (*clk_enable)(struct tpm_chip *, bool);
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
<code>unsigned int flags</code>
</li>
</ul>
</details>
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
<code>int (*request_locality)(struct tpm_chip *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*relinquish_locality)(struct tpm_chip *, int)</code>
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
<code>void (*clk_enable)(struct tpm_chip *, bool)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*go_idle)(struct tpm_chip *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*cmd_ready)(struct tpm_chip *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*relinquish_locality)(struct tpm_chip *, int)</code> ➡️ <code>int (*relinquish_locality)(struct tpm_chip *, int)</code>
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
<b>Field type changed. </b>
<code>bool (*update_timeouts)(struct tpm_chip *, long unsigned int *)</code> ➡️ <code>void (*update_timeouts)(struct tpm_chip *, long unsigned int *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*update_durations)(struct tpm_chip *, long unsigned int *)</code>
</li>
</ul>
</details>
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
