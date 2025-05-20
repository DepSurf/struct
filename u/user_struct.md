# Struct: <code>user_struct</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct user_struct {
    atomic_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t inotify_watches;
    atomic_t inotify_devs;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct key *uid_keyring;
    struct key *session_keyring;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct user_struct {
    atomic_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t inotify_watches;
    atomic_t inotify_devs;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct key *uid_keyring;
    struct key *session_keyring;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct user_struct {
    atomic_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t inotify_watches;
    atomic_t inotify_devs;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct key *uid_keyring;
    struct key *session_keyring;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct user_struct {
    atomic_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct key *uid_keyring;
    struct key *session_keyring;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct user_struct {
    atomic_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct key *uid_keyring;
    struct key *session_keyring;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct user_struct {
    atomic_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct key *uid_keyring;
    struct key *session_keyring;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct key *uid_keyring;
    struct key *session_keyring;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    struct percpu_counter epoll_watches;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    struct percpu_counter epoll_watches;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    struct percpu_counter epoll_watches;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    struct percpu_counter epoll_watches;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    struct percpu_counter epoll_watches;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    atomic_t nr_watches;
    struct ratelimit_state ratelimit;
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
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
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
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct user_struct {
    refcount_t __count;
    atomic_t processes;
    atomic_t sigpending;
    atomic_t fanotify_listeners;
    atomic_long_t epoll_watches;
    long unsigned int mq_bytes;
    long unsigned int locked_shm;
    long unsigned int unix_inflight;
    atomic_long_t pipe_bufs;
    struct hlist_node uidhash_node;
    kuid_t uid;
    atomic_long_t locked_vm;
    struct ratelimit_state ratelimit;
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t inotify_watches</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t inotify_devs</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ratelimit_state ratelimit</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t __count</code> ➡️ <code>refcount_t __count</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct key *uid_keyring</code>
</li>
<li>
<b>Field removed. </b>
<code>struct key *session_keyring</code>
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
<code>atomic_t nr_watches</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.8</code> and <code>5.11</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t fanotify_listeners</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>atomic_t processes</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t sigpending</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int mq_bytes</code>
</li>
<li>
<b>Field removed. </b>
<code>long unsigned int locked_shm</code>
</li>
<li>
<b>Field type changed. </b>
<code>atomic_long_t epoll_watches</code> ➡️ <code>struct percpu_counter epoll_watches</code>
</li>
</ul>
</details>
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
