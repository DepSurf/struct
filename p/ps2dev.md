# Struct: <code>ps2dev</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    unsigned char cmdbuf[8];
    unsigned char cmdcnt;
    unsigned char nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    unsigned char cmdbuf[8];
    unsigned char cmdcnt;
    unsigned char nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    unsigned char cmdbuf[8];
    unsigned char cmdcnt;
    unsigned char nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    unsigned char cmdbuf[8];
    unsigned char cmdcnt;
    unsigned char nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    unsigned char cmdbuf[8];
    unsigned char cmdcnt;
    unsigned char nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
    ps2_pre_receive_handler_t pre_receive_handler;
    ps2_receive_handler_t receive_handler;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
    ps2_pre_receive_handler_t pre_receive_handler;
    ps2_receive_handler_t receive_handler;
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
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
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
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ps2dev {
    struct serio *serio;
    struct mutex cmd_mutex;
    wait_queue_head_t wait;
    long unsigned int flags;
    u8 cmdbuf[8];
    u8 cmdcnt;
    u8 nak;
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
<code>unsigned char cmdbuf[8]</code> ➡️ <code>u8 cmdbuf[8]</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char cmdcnt</code> ➡️ <code>u8 cmdcnt</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned char nak</code> ➡️ <code>u8 nak</code>
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
<code>ps2_pre_receive_handler_t pre_receive_handler</code>
</li>
<li>
<b>Field added. </b>
<code>ps2_receive_handler_t receive_handler</code>
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
