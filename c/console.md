# Struct: <code>console</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    uint ispeed;
    uint ospeed;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    uint ispeed;
    uint ospeed;
    u64 seq;
    long unsigned int dropped;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    uint ispeed;
    uint ospeed;
    u64 seq;
    long unsigned int dropped;
    void *data;
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    uint ispeed;
    uint ospeed;
    u64 seq;
    long unsigned int dropped;
    void *data;
    struct hlist_node node;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*exit)(struct console *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    uint ispeed;
    uint ospeed;
    u64 seq;
    long unsigned int dropped;
    void *data;
    struct hlist_node node;
    bool (*write_atomic)(struct console *, struct nbcon_write_context *);
    atomic_t nbcon_state;
    atomic_long_t nbcon_seq;
    struct printk_buffers *pbufs;
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
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
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
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct console {
    char name[16];
    void (*write)(struct console *, const char *, unsigned int);
    int (*read)(struct console *, char *, unsigned int);
    struct tty_driver * (*device)(struct console *, int *);
    void (*unblank)();
    int (*setup)(struct console *, char *);
    int (*match)(struct console *, char *, int, char *);
    short int flags;
    short int index;
    int cflag;
    void *data;
    struct console *next;
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
<b>Field added. </b>
<code>int (*exit)(struct console *)</code>
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>uint ispeed</code>
</li>
<li>
<b>Field added. </b>
<code>uint ospeed</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u64 seq</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int dropped</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct hlist_node node</code>
</li>
<li>
<b>Field removed. </b>
<code>struct console *next</code>
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
<b>Field added. </b>
<code>bool (*write_atomic)(struct console *, struct nbcon_write_context *)</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_t nbcon_state</code>
</li>
<li>
<b>Field added. </b>
<code>atomic_long_t nbcon_seq</code>
</li>
<li>
<b>Field added. </b>
<code>struct printk_buffers *pbufs</code>
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
