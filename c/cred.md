# Struct: <code>cred</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cred {
    atomic_long_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct ucounts *ucounts;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
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
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
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
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cred {
    atomic_t usage;
    kuid_t uid;
    kgid_t gid;
    kuid_t suid;
    kgid_t sgid;
    kuid_t euid;
    kgid_t egid;
    kuid_t fsuid;
    kgid_t fsgid;
    unsigned int securebits;
    kernel_cap_t cap_inheritable;
    kernel_cap_t cap_permitted;
    kernel_cap_t cap_effective;
    kernel_cap_t cap_bset;
    kernel_cap_t cap_ambient;
    unsigned char jit_keyring;
    struct key *session_keyring;
    struct key *process_keyring;
    struct key *thread_keyring;
    struct key *request_key_auth;
    void *security;
    struct user_struct *user;
    struct user_namespace *user_ns;
    struct group_info *group_info;
    int non_rcu;
    struct callback_head rcu;
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
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int non_rcu</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ucounts *ucounts</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>atomic_t usage</code> ➡️ <code>atomic_long_t usage</code>
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
