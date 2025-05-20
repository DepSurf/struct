# Struct: <code>acpi_button</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
    bool lid_state_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
    bool lid_state_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
    bool lid_state_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
    bool lid_state_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
    bool lid_state_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
    bool lid_state_initialized;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
    bool lid_state_initialized;
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
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
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
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct acpi_button {
    unsigned int type;
    struct input_dev *input;
    char phys[32];
    long unsigned int pushed;
    int last_state;
    ktime_t last_time;
    bool suspended;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int last_state</code>
</li>
<li>
<b>Field added. </b>
<code>ktime_t last_time</code>
</li>
</ul>
</details>
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
No changes between <code>5.4</code> and <code>5.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool lid_state_initialized</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
