# Struct: <code>uinput_device</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
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
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
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
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct uinput_device {
    struct input_dev *dev;
    struct mutex mutex;
    enum uinput_state state;
    wait_queue_head_t waitq;
    unsigned char ready;
    unsigned char head;
    unsigned char tail;
    struct input_event buff[16];
    unsigned int ff_effects_max;
    struct uinput_request * requests[16];
    wait_queue_head_t requests_waitq;
    spinlock_t requests_lock;
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
