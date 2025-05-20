# Struct: <code>evtchn_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    bool (*test_and_set_mask)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(evtchn_port_t);
    void (*remove)(evtchn_port_t, unsigned int);
    void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *);
    void (*resume)();
    int (*percpu_init)(unsigned int);
    int (*percpu_deinit)(unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(evtchn_port_t);
    void (*remove)(evtchn_port_t, unsigned int);
    void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *);
    void (*resume)();
    int (*percpu_init)(unsigned int);
    int (*percpu_deinit)(unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(evtchn_port_t);
    void (*remove)(evtchn_port_t, unsigned int);
    void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *);
    void (*resume)();
    int (*percpu_init)(unsigned int);
    int (*percpu_deinit)(unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(evtchn_port_t);
    void (*remove)(evtchn_port_t, unsigned int);
    void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *);
    void (*resume)();
    int (*percpu_init)(unsigned int);
    int (*percpu_deinit)(unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(evtchn_port_t);
    void (*remove)(evtchn_port_t, unsigned int);
    void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *);
    void (*resume)();
    int (*percpu_init)(unsigned int);
    int (*percpu_deinit)(unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(evtchn_port_t);
    void (*remove)(evtchn_port_t, unsigned int);
    void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *);
    void (*resume)();
    int (*percpu_init)(unsigned int);
    int (*percpu_deinit)(unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(evtchn_port_t);
    void (*remove)(evtchn_port_t, unsigned int);
    void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int);
    void (*clear_pending)(evtchn_port_t);
    void (*set_pending)(evtchn_port_t);
    bool (*is_pending)(evtchn_port_t);
    void (*mask)(evtchn_port_t);
    void (*unmask)(evtchn_port_t);
    void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *);
    void (*resume)();
    int (*percpu_init)(unsigned int);
    int (*percpu_deinit)(unsigned int);
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
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
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
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
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
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct evtchn_ops {
    unsigned int (*max_channels)();
    unsigned int (*nr_channels)();
    int (*setup)(struct irq_info *);
    void (*bind_to_cpu)(struct irq_info *, unsigned int);
    void (*clear_pending)(unsigned int);
    void (*set_pending)(unsigned int);
    bool (*is_pending)(unsigned int);
    bool (*test_and_set_mask)(unsigned int);
    void (*mask)(unsigned int);
    void (*unmask)(unsigned int);
    void (*handle_events)(unsigned int);
    void (*resume)();
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
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
No changes between <code>5.0</code> and <code>5.3</code> ✅
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>void (*clear_pending)(unsigned int)</code> ➡️ <code>void (*clear_pending)(evtchn_port_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*set_pending)(unsigned int)</code> ➡️ <code>void (*set_pending)(evtchn_port_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*is_pending)(unsigned int)</code> ➡️ <code>bool (*is_pending)(evtchn_port_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>bool (*test_and_set_mask)(unsigned int)</code> ➡️ <code>bool (*test_and_set_mask)(evtchn_port_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*mask)(unsigned int)</code> ➡️ <code>void (*mask)(evtchn_port_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*unmask)(unsigned int)</code> ➡️ <code>void (*unmask)(evtchn_port_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*remove)(evtchn_port_t, unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*percpu_init)(unsigned int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*percpu_deinit)(unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*test_and_set_mask)(evtchn_port_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*setup)(struct irq_info *)</code> ➡️ <code>int (*setup)(evtchn_port_t)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*bind_to_cpu)(struct irq_info *, unsigned int)</code> ➡️ <code>void (*bind_to_cpu)(evtchn_port_t, unsigned int, unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*handle_events)(unsigned int)</code> ➡️ <code>void (*handle_events)(unsigned int, struct evtchn_loop_ctrl *)</code>
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
