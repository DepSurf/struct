# Struct: <code>deflate_state</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
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
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
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
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct deflate_state {
    z_streamp strm;
    int status;
    Byte *pending_buf;
    ulg pending_buf_size;
    Byte *pending_out;
    int pending;
    int noheader;
    Byte data_type;
    Byte method;
    int last_flush;
    uInt w_size;
    uInt w_bits;
    uInt w_mask;
    Byte *window;
    ulg window_size;
    Pos *prev;
    Pos *head;
    uInt ins_h;
    uInt hash_size;
    uInt hash_bits;
    uInt hash_mask;
    uInt hash_shift;
    long int block_start;
    uInt match_length;
    IPos prev_match;
    int match_available;
    uInt strstart;
    uInt match_start;
    uInt lookahead;
    uInt prev_length;
    uInt max_chain_length;
    uInt max_lazy_match;
    int level;
    int strategy;
    uInt good_match;
    int nice_match;
    struct ct_data_s dyn_ltree[573];
    struct ct_data_s dyn_dtree[61];
    struct ct_data_s bl_tree[39];
    struct tree_desc_s l_desc;
    struct tree_desc_s d_desc;
    struct tree_desc_s bl_desc;
    ush bl_count[16];
    int heap[573];
    int heap_len;
    int heap_max;
    uch depth[573];
    uch *l_buf;
    uInt lit_bufsize;
    uInt last_lit;
    ush *d_buf;
    ulg opt_len;
    ulg static_len;
    ulg compressed_len;
    uInt matches;
    int last_eob_len;
    ush bi_buf;
    int bi_valid;
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
