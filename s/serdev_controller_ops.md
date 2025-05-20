# Struct: <code>serdev_controller_ops</code>

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
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
    int (*break_ctl)(struct serdev_controller *, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct serdev_controller_ops {
    ssize_t (*write_buf)(struct serdev_controller *, const u8 *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
    int (*break_ctl)(struct serdev_controller *, unsigned int);
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
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
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
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
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
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct serdev_controller_ops {
    int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t);
    void (*write_flush)(struct serdev_controller *);
    int (*write_room)(struct serdev_controller *);
    int (*open)(struct serdev_controller *);
    void (*close)(struct serdev_controller *);
    void (*set_flow_control)(struct serdev_controller *, bool);
    int (*set_parity)(struct serdev_controller *, enum serdev_parity);
    unsigned int (*set_baudrate)(struct serdev_controller *, unsigned int);
    void (*wait_until_sent)(struct serdev_controller *, long int);
    int (*get_tiocm)(struct serdev_controller *);
    int (*set_tiocm)(struct serdev_controller *, unsigned int, unsigned int);
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*set_parity)(struct serdev_controller *, enum serdev_parity)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*break_ctl)(struct serdev_controller *, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*write_buf)(struct serdev_controller *, const unsigned char *, size_t)</code> ➡️ <code>ssize_t (*write_buf)(struct serdev_controller *, const u8 *, size_t)</code>
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
