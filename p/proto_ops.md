# Struct: <code>proto_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int);
    int (*getname)(struct socket *, struct sockaddr *, int *, int);
    unsigned int (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int);
    int (*getname)(struct socket *, struct sockaddr *, int *, int);
    unsigned int (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int);
    int (*getname)(struct socket *, struct sockaddr *, int *, int);
    unsigned int (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int *, int);
    unsigned int (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int *, int);
    unsigned int (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    unsigned int flags;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*read_skb)(struct sock *, skb_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    void (*splice_eof)(struct socket *);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*read_skb)(struct sock *, skb_read_actor_t);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    void (*show_fdinfo)(struct seq_file *, struct socket *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    void (*splice_eof)(struct socket *);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*read_skb)(struct sock *, skb_read_actor_t);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
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
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
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
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct proto_ops {
    int family;
    struct module *owner;
    int (*release)(struct socket *);
    int (*bind)(struct socket *, struct sockaddr *, int);
    int (*connect)(struct socket *, struct sockaddr *, int, int);
    int (*socketpair)(struct socket *, struct socket *);
    int (*accept)(struct socket *, struct socket *, int, bool);
    int (*getname)(struct socket *, struct sockaddr *, int);
    __poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *);
    int (*ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int);
    int (*gettstamp)(struct socket *, void *, bool, bool);
    int (*listen)(struct socket *, int);
    int (*shutdown)(struct socket *, int);
    int (*setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*getsockopt)(struct socket *, int, int, char *, int *);
    int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int);
    int (*compat_getsockopt)(struct socket *, int, int, char *, int *);
    int (*sendmsg)(struct socket *, struct msghdr *, size_t);
    int (*recvmsg)(struct socket *, struct msghdr *, size_t, int);
    int (*mmap)(struct file *, struct socket *, struct vm_area_struct *);
    ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int);
    ssize_t (*splice_read)(struct socket *, loff_t *, struct pipe_inode_info *, size_t, unsigned int);
    int (*set_peek_off)(struct sock *, int);
    int (*peek_len)(struct socket *);
    int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t);
    int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int);
    int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t);
    int (*set_rcvlowat)(struct sock *, int);
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
<code>int (*peek_len)(struct socket *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*read_sock)(struct sock *, read_descriptor_t *, sk_read_actor_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*accept)(struct socket *, struct socket *, int)</code> ➡️ <code>int (*accept)(struct socket *, struct socket *, int, bool)</code>
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
<code>int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*sendmsg_locked)(struct sock *, struct msghdr *, size_t)</code>
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
<code>int (*set_rcvlowat)(struct sock *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*getname)(struct socket *, struct sockaddr *, int *, int)</code> ➡️ <code>int (*getname)(struct socket *, struct sockaddr *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>unsigned int (*poll)(struct file *, struct socket *, struct poll_table_struct *)</code> ➡️ <code>__poll_t (*poll)(struct file *, struct socket *, struct poll_table_struct *)</code>
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
<b>Field added. </b>
<code>int (*gettstamp)(struct socket *, void *, bool, bool)</code>
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
<code>void (*show_fdinfo)(struct seq_file *, struct socket *)</code>
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
<code>unsigned int flags</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct socket *, int, int, char *, int *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*setsockopt)(struct socket *, int, int, char *, unsigned int)</code> ➡️ <code>int (*setsockopt)(struct socket *, int, int, sockptr_t, unsigned int)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>unsigned int flags</code>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*read_skb)(struct sock *, skb_read_actor_t)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*splice_eof)(struct socket *)</code>
</li>
<li>
<b>Field removed. </b>
<code>ssize_t (*sendpage)(struct socket *, struct page *, int, size_t, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*sendpage_locked)(struct sock *, struct page *, int, size_t, int)</code>
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
<details>
<summary>Changed between <code>amd64</code> and <code>armhf</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct socket *, int, int, char *, int *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>amd64</code> and <code>ppc64el</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>amd64</code> and <code>riscv64</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*compat_ioctl)(struct socket *, unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_setsockopt)(struct socket *, int, int, char *, unsigned int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*compat_getsockopt)(struct socket *, int, int, char *, int *)</code>
</li>
</ul>
</details>
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
