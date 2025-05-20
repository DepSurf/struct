# Struct: <code>clk_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    void (*init)(struct clk_hw *);
    int (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    void (*init)(struct clk_hw *);
    int (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    void (*init)(struct clk_hw *);
    int (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    void (*init)(struct clk_hw *);
    int (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    void (*init)(struct clk_hw *);
    int (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*init)(struct clk_hw *);
    void (*terminate)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
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
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
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
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct clk_ops {
    int (*prepare)(struct clk_hw *);
    void (*unprepare)(struct clk_hw *);
    int (*is_prepared)(struct clk_hw *);
    void (*unprepare_unused)(struct clk_hw *);
    int (*enable)(struct clk_hw *);
    void (*disable)(struct clk_hw *);
    int (*is_enabled)(struct clk_hw *);
    void (*disable_unused)(struct clk_hw *);
    int (*save_context)(struct clk_hw *);
    void (*restore_context)(struct clk_hw *);
    long unsigned int (*recalc_rate)(struct clk_hw *, long unsigned int);
    long int (*round_rate)(struct clk_hw *, long unsigned int, long unsigned int *);
    int (*determine_rate)(struct clk_hw *, struct clk_rate_request *);
    int (*set_parent)(struct clk_hw *, u8);
    u8 (*get_parent)(struct clk_hw *);
    int (*set_rate)(struct clk_hw *, long unsigned int, long unsigned int);
    int (*set_rate_and_parent)(struct clk_hw *, long unsigned int, long unsigned int, u8);
    long unsigned int (*recalc_accuracy)(struct clk_hw *, long unsigned int);
    int (*get_phase)(struct clk_hw *);
    int (*set_phase)(struct clk_hw *, int);
    int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *);
    int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *);
    void (*init)(struct clk_hw *);
    void (*debug_init)(struct clk_hw *, struct dentry *);
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*debug_init)(struct clk_hw *, struct dentry *)</code> ➡️ <code>void (*debug_init)(struct clk_hw *, struct dentry *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*save_context)(struct clk_hw *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*restore_context)(struct clk_hw *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_duty_cycle)(struct clk_hw *, struct clk_duty *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*set_duty_cycle)(struct clk_hw *, struct clk_duty *)</code>
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
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*terminate)(struct clk_hw *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*init)(struct clk_hw *)</code> ➡️ <code>int (*init)(struct clk_hw *)</code>
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
