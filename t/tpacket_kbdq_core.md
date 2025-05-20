# Struct: <code>tpacket_kbdq_core</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    rwlock_t blk_fill_in_prog_lock;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    rwlock_t blk_fill_in_prog_lock;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    rwlock_t blk_fill_in_prog_lock;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    rwlock_t blk_fill_in_prog_lock;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    rwlock_t blk_fill_in_prog_lock;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    rwlock_t blk_fill_in_prog_lock;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    rwlock_t blk_fill_in_prog_lock;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
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
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
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
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct tpacket_kbdq_core {
    struct pgv *pkbdq;
    unsigned int feature_req_word;
    unsigned int hdrlen;
    unsigned char reset_pending_on_curr_blk;
    unsigned char delete_blk_timer;
    short unsigned int kactive_blk_num;
    short unsigned int blk_sizeof_priv;
    short unsigned int last_kactive_blk_num;
    char *pkblk_start;
    char *pkblk_end;
    int kblk_size;
    unsigned int max_frame_len;
    unsigned int knum_blocks;
    uint64_t knxt_seq_num;
    char *prev;
    char *nxt_offset;
    struct sk_buff *skb;
    atomic_t blk_fill_in_prog;
    short unsigned int retire_blk_tov;
    short unsigned int version;
    long unsigned int tov_in_jiffies;
    struct timer_list retire_blk_timer;
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>rwlock_t blk_fill_in_prog_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>atomic_t blk_fill_in_prog</code>
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
