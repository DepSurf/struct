# Struct: <code>bpf_map_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct bpf_map_ops {
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, int);
    void (*map_fd_put_ptr)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct bpf_map_ops {
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct bpf_map_ops {
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct bpf_map_ops {
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct bpf_map_ops {
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, u32, u32);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
    int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32);
    void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32);
    struct bpf_local_storage ** (*map_owner_storage_ptr)(void *);
    bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *);
    const const char * map_btf_name;
    int *map_btf_id;
    const struct bpf_iter_seq_info *iter_seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
    int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32);
    void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32);
    struct bpf_local_storage ** (*map_owner_storage_ptr)(void *);
    int (*map_redirect)(struct bpf_map *, u32, u64);
    bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *);
    int (*map_set_for_each_callback_args)(struct bpf_verifier_env *, struct bpf_func_state *, struct bpf_func_state *);
    int (*map_for_each_callback)(struct bpf_map *, void *, void *, u64);
    const const char * map_btf_name;
    int *map_btf_id;
    const struct bpf_iter_seq_info *iter_seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
    int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32);
    void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32);
    struct bpf_local_storage ** (*map_owner_storage_ptr)(void *);
    int (*map_redirect)(struct bpf_map *, u32, u64);
    bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *);
    int (*map_set_for_each_callback_args)(struct bpf_verifier_env *, struct bpf_func_state *, struct bpf_func_state *);
    int (*map_for_each_callback)(struct bpf_map *, void *, void *, u64);
    const const char * map_btf_name;
    int *map_btf_id;
    const struct bpf_iter_seq_info *iter_seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_lookup_percpu_elem)(struct bpf_map *, void *, u32);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
    int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32);
    void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32);
    struct bpf_local_storage ** (*map_owner_storage_ptr)(void *);
    int (*map_redirect)(struct bpf_map *, u32, u64);
    bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *);
    int (*map_set_for_each_callback_args)(struct bpf_verifier_env *, struct bpf_func_state *, struct bpf_func_state *);
    int (*map_for_each_callback)(struct bpf_map *, bpf_callback_t, void *, u64);
    int *map_btf_id;
    const struct bpf_iter_seq_info *iter_seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, struct file *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_lookup_percpu_elem)(struct bpf_map *, void *, u32);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
    int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32);
    void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32);
    struct bpf_local_storage ** (*map_owner_storage_ptr)(void *);
    int (*map_redirect)(struct bpf_map *, u64, u64);
    bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *);
    int (*map_set_for_each_callback_args)(struct bpf_verifier_env *, struct bpf_func_state *, struct bpf_func_state *);
    int (*map_for_each_callback)(struct bpf_map *, bpf_callback_t, void *, u64);
    int *map_btf_id;
    const struct bpf_iter_seq_info *iter_seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, struct file *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    long int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    long int (*map_delete_elem)(struct bpf_map *, void *);
    long int (*map_push_elem)(struct bpf_map *, void *, u64);
    long int (*map_pop_elem)(struct bpf_map *, void *);
    long int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_lookup_percpu_elem)(struct bpf_map *, void *, u32);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
    int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32);
    void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32);
    struct bpf_local_storage ** (*map_owner_storage_ptr)(void *);
    long int (*map_redirect)(struct bpf_map *, u64, u64);
    bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *);
    int (*map_set_for_each_callback_args)(struct bpf_verifier_env *, struct bpf_func_state *, struct bpf_func_state *);
    long int (*map_for_each_callback)(struct bpf_map *, bpf_callback_t, void *, u64);
    u64 (*map_mem_usage)(const struct bpf_map *);
    int *map_btf_id;
    const struct bpf_iter_seq_info *iter_seq_info;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_lookup_and_delete_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    int (*map_update_batch)(struct bpf_map *, struct file *, const union bpf_attr *, union bpf_attr *);
    int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    long int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    long int (*map_delete_elem)(struct bpf_map *, void *);
    long int (*map_push_elem)(struct bpf_map *, void *, u64);
    long int (*map_pop_elem)(struct bpf_map *, void *);
    long int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_lookup_percpu_elem)(struct bpf_map *, void *, u32);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(struct bpf_map *, void *, bool);
    int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *);
    void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
    int (*map_mmap)(struct bpf_map *, struct vm_area_struct *);
    __poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *);
    int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32);
    void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32);
    struct bpf_local_storage ** (*map_owner_storage_ptr)(void *);
    long int (*map_redirect)(struct bpf_map *, u64, u64);
    bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *);
    int (*map_set_for_each_callback_args)(struct bpf_verifier_env *, struct bpf_func_state *, struct bpf_func_state *);
    long int (*map_for_each_callback)(struct bpf_map *, bpf_callback_t, void *, u64);
    u64 (*map_mem_usage)(const struct bpf_map *);
    int *map_btf_id;
    const struct bpf_iter_seq_info *iter_seq_info;
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
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
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
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct bpf_map_ops {
    int (*map_alloc_check)(union bpf_attr *);
    struct bpf_map * (*map_alloc)(union bpf_attr *);
    void (*map_release)(struct bpf_map *, struct file *);
    void (*map_free)(struct bpf_map *);
    int (*map_get_next_key)(struct bpf_map *, void *, void *);
    void (*map_release_uref)(struct bpf_map *);
    void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *);
    void * (*map_lookup_elem)(struct bpf_map *, void *);
    int (*map_update_elem)(struct bpf_map *, void *, void *, u64);
    int (*map_delete_elem)(struct bpf_map *, void *);
    int (*map_push_elem)(struct bpf_map *, void *, u64);
    int (*map_pop_elem)(struct bpf_map *, void *);
    int (*map_peek_elem)(struct bpf_map *, void *);
    void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int);
    void (*map_fd_put_ptr)(void *);
    u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *);
    u32 (*map_fd_sys_lookup_elem)(void *);
    void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *);
    int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *);
    int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32);
    int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *);
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
<code>void (*map_release)(struct bpf_map *, struct file *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void * (*map_fd_get_ptr)(struct bpf_map *, int)</code> ➡️ <code>void * (*map_fd_get_ptr)(struct bpf_map *, struct file *, int)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *)</code>
</li>
<li>
<b>Field added. </b>
<code>u32 (*map_fd_sys_lookup_elem)(void *)</code>
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
<code>int (*map_alloc_check)(union bpf_attr *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*map_release_uref)(struct bpf_map *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*map_seq_show_elem)(struct bpf_map *, void *, struct seq_file *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_check_btf)(const struct bpf_map *, const struct btf *, u32, u32)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*map_push_elem)(struct bpf_map *, void *, u64)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_pop_elem)(struct bpf_map *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_peek_elem)(struct bpf_map *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_check_btf)(const struct bpf_map *, const struct btf *, u32, u32)</code> ➡️ <code>int (*map_check_btf)(const struct bpf_map *, const struct btf *, const struct btf_type *, const struct btf_type *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void * (*map_lookup_elem_sys_only)(struct bpf_map *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_direct_value_addr)(const struct bpf_map *, u64 *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_direct_value_meta)(const struct bpf_map *, u64, u32 *)</code>
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
<code>int (*map_lookup_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_lookup_and_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_update_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_delete_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_poke_track)(struct bpf_map *, struct bpf_prog_aux *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*map_poke_untrack)(struct bpf_map *, struct bpf_prog_aux *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*map_poke_run)(struct bpf_map *, u32, struct bpf_prog *, struct bpf_prog *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_mmap)(struct bpf_map *, struct vm_area_struct *)</code>
</li>
<li>
<b>Field added. </b>
<code>__poll_t (*map_poll)(struct bpf_map *, struct file *, struct poll_table_struct *)</code>
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
<code>int (*map_local_storage_charge)(struct bpf_local_storage_map *, void *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*map_local_storage_uncharge)(struct bpf_local_storage_map *, void *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>struct bpf_local_storage ** (*map_owner_storage_ptr)(void *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*map_meta_equal)(const struct bpf_map *, const struct bpf_map *)</code>
</li>
<li>
<b>Field added. </b>
<code>const const char * map_btf_name</code>
</li>
<li>
<b>Field added. </b>
<code>int *map_btf_id</code>
</li>
<li>
<b>Field added. </b>
<code>const struct bpf_iter_seq_info *iter_seq_info</code>
</li>
<li>
<b>Field type changed. </b>
<code>u32 (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *)</code> ➡️ <code>int (*map_gen_lookup)(struct bpf_map *, struct bpf_insn *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*map_redirect)(struct bpf_map *, u32, u64)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_set_for_each_callback_args)(struct bpf_verifier_env *, struct bpf_func_state *, struct bpf_func_state *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_for_each_callback)(struct bpf_map *, void *, void *, u64)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*map_lookup_and_delete_elem)(struct bpf_map *, void *, void *, u64)</code>
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
<code>void * (*map_lookup_percpu_elem)(struct bpf_map *, void *, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>const const char * map_btf_name</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_for_each_callback)(struct bpf_map *, void *, void *, u64)</code> ➡️ <code>int (*map_for_each_callback)(struct bpf_map *, bpf_callback_t, void *, u64)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*map_update_batch)(struct bpf_map *, const union bpf_attr *, union bpf_attr *)</code> ➡️ <code>int (*map_update_batch)(struct bpf_map *, struct file *, const union bpf_attr *, union bpf_attr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_redirect)(struct bpf_map *, u32, u64)</code> ➡️ <code>int (*map_redirect)(struct bpf_map *, u64, u64)</code>
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
<code>u64 (*map_mem_usage)(const struct bpf_map *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_update_elem)(struct bpf_map *, void *, void *, u64)</code> ➡️ <code>long int (*map_update_elem)(struct bpf_map *, void *, void *, u64)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_delete_elem)(struct bpf_map *, void *)</code> ➡️ <code>long int (*map_delete_elem)(struct bpf_map *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_push_elem)(struct bpf_map *, void *, u64)</code> ➡️ <code>long int (*map_push_elem)(struct bpf_map *, void *, u64)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_pop_elem)(struct bpf_map *, void *)</code> ➡️ <code>long int (*map_pop_elem)(struct bpf_map *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_peek_elem)(struct bpf_map *, void *)</code> ➡️ <code>long int (*map_peek_elem)(struct bpf_map *, void *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_redirect)(struct bpf_map *, u64, u64)</code> ➡️ <code>long int (*map_redirect)(struct bpf_map *, u64, u64)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*map_for_each_callback)(struct bpf_map *, bpf_callback_t, void *, u64)</code> ➡️ <code>long int (*map_for_each_callback)(struct bpf_map *, bpf_callback_t, void *, u64)</code>
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
<code>void (*map_fd_put_ptr)(void *)</code> ➡️ <code>void (*map_fd_put_ptr)(struct bpf_map *, void *, bool)</code>
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
