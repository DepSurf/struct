# Struct: <code>devlink_ops</code>

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
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct devlink_ops {
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int);
    int (*port_unsplit)(struct devlink *, unsigned int);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8);
    int (*eswitch_encap_mode_get)(struct devlink *, u8 *);
    int (*eswitch_encap_mode_set)(struct devlink *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct devlink_ops {
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int);
    int (*port_unsplit)(struct devlink *, unsigned int);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8);
    int (*eswitch_encap_mode_get)(struct devlink *, u8 *);
    int (*eswitch_encap_mode_set)(struct devlink *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8);
    int (*eswitch_encap_mode_get)(struct devlink *, u8 *);
    int (*eswitch_encap_mode_set)(struct devlink *, u8);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, u8 *);
    int (*eswitch_encap_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, bool, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct devlink_ops {
    u32 supported_flash_update_params;
    long unsigned int reload_actions;
    long unsigned int reload_limits;
    int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *);
    int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
    int (*port_function_hw_addr_get)(struct devlink *, struct devlink_port *, u8 *, int *, struct netlink_ext_ack *);
    int (*port_function_hw_addr_set)(struct devlink *, struct devlink_port *, const u8 *, int, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct devlink_ops {
    u32 supported_flash_update_params;
    long unsigned int reload_actions;
    long unsigned int reload_limits;
    int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *);
    int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
    int (*port_function_hw_addr_get)(struct devlink *, struct devlink_port *, u8 *, int *, struct netlink_ext_ack *);
    int (*port_function_hw_addr_set)(struct devlink *, struct devlink_port *, const u8 *, int, struct netlink_ext_ack *);
    int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, unsigned int *);
    int (*port_del)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*port_fn_state_get)(struct devlink *, struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *);
    int (*port_fn_state_set)(struct devlink *, struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct devlink_ops {
    u32 supported_flash_update_params;
    long unsigned int reload_actions;
    long unsigned int reload_limits;
    int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *);
    int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_drop_counter_get)(struct devlink *, const struct devlink_trap *, u64 *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
    int (*port_function_hw_addr_get)(struct devlink_port *, u8 *, int *, struct netlink_ext_ack *);
    int (*port_function_hw_addr_set)(struct devlink_port *, const u8 *, int, struct netlink_ext_ack *);
    int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, unsigned int *);
    int (*port_del)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*port_fn_state_get)(struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *);
    int (*port_fn_state_set)(struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *);
    int (*rate_leaf_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_new)(struct devlink_rate *, void **, struct netlink_ext_ack *);
    int (*rate_node_del)(struct devlink_rate *, void *, struct netlink_ext_ack *);
    int (*rate_leaf_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    int (*rate_node_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct devlink_ops {
    u32 supported_flash_update_params;
    long unsigned int reload_actions;
    long unsigned int reload_limits;
    int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, struct devlink_port *, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *);
    int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_drop_counter_get)(struct devlink *, const struct devlink_trap *, u64 *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
    int (*port_function_hw_addr_get)(struct devlink_port *, u8 *, int *, struct netlink_ext_ack *);
    int (*port_function_hw_addr_set)(struct devlink_port *, const u8 *, int, struct netlink_ext_ack *);
    int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, unsigned int *);
    int (*port_del)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*port_fn_state_get)(struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *);
    int (*port_fn_state_set)(struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *);
    int (*rate_leaf_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_new)(struct devlink_rate *, void **, struct netlink_ext_ack *);
    int (*rate_node_del)(struct devlink_rate *, void *, struct netlink_ext_ack *);
    int (*rate_leaf_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    int (*rate_node_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct devlink_ops {
    u32 supported_flash_update_params;
    long unsigned int reload_actions;
    long unsigned int reload_limits;
    int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, struct devlink_port *, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *);
    int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_drop_counter_get)(struct devlink *, const struct devlink_trap *, u64 *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
    int (*port_function_hw_addr_get)(struct devlink_port *, u8 *, int *, struct netlink_ext_ack *);
    int (*port_function_hw_addr_set)(struct devlink_port *, const u8 *, int, struct netlink_ext_ack *);
    int (*port_fn_roce_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_roce_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
    int (*port_fn_migratable_get)(struct devlink_port *, bool *, struct netlink_ext_ack *);
    int (*port_fn_migratable_set)(struct devlink_port *, bool, struct netlink_ext_ack *);
    int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, unsigned int *);
    int (*port_del)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*port_fn_state_get)(struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *);
    int (*port_fn_state_set)(struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *);
    int (*rate_leaf_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_leaf_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_new)(struct devlink_rate *, void **, struct netlink_ext_ack *);
    int (*rate_node_del)(struct devlink_rate *, void *, struct netlink_ext_ack *);
    int (*rate_leaf_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    int (*rate_node_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    bool (*selftest_check)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    enum devlink_selftest_status (*selftest_run)(struct devlink *, unsigned int, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct devlink_ops {
    u32 supported_flash_update_params;
    long unsigned int reload_actions;
    long unsigned int reload_limits;
    int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *);
    int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_drop_counter_get)(struct devlink *, const struct devlink_trap *, u64 *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
    int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, struct devlink_port **);
    int (*rate_leaf_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_leaf_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_new)(struct devlink_rate *, void **, struct netlink_ext_ack *);
    int (*rate_node_del)(struct devlink_rate *, void *, struct netlink_ext_ack *);
    int (*rate_leaf_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    int (*rate_node_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    bool (*selftest_check)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    enum devlink_selftest_status (*selftest_run)(struct devlink *, unsigned int, struct netlink_ext_ack *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct devlink_ops {
    u32 supported_flash_update_params;
    long unsigned int reload_actions;
    long unsigned int reload_limits;
    int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
    int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *);
    int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *);
    int (*trap_drop_counter_get)(struct devlink *, const struct devlink_trap *, u64 *);
    int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *);
    void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *);
    int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *);
    int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *);
    int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, struct devlink_port **);
    int (*rate_leaf_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_leaf_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_leaf_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *);
    int (*rate_node_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *);
    int (*rate_node_new)(struct devlink_rate *, void **, struct netlink_ext_ack *);
    int (*rate_node_del)(struct devlink_rate *, void *, struct netlink_ext_ack *);
    int (*rate_leaf_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    int (*rate_node_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *);
    bool (*selftest_check)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    enum devlink_selftest_status (*selftest_run)(struct devlink *, unsigned int, struct netlink_ext_ack *);
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
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
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
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct devlink_ops {
    int (*reload_down)(struct devlink *, struct netlink_ext_ack *);
    int (*reload_up)(struct devlink *, struct netlink_ext_ack *);
    int (*port_type_set)(struct devlink_port *, enum devlink_port_type);
    int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *);
    int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *);
    int (*sb_pool_get)(struct devlink *, unsigned int, u16, struct devlink_sb_pool_info *);
    int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *);
    int (*sb_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *);
    int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *);
    int (*sb_tc_pool_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16 *, u32 *);
    int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *);
    int (*sb_occ_snapshot)(struct devlink *, unsigned int);
    int (*sb_occ_max_clear)(struct devlink *, unsigned int);
    int (*sb_occ_port_pool_get)(struct devlink_port *, unsigned int, u16, u32 *, u32 *);
    int (*sb_occ_tc_port_bind_get)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u32 *, u32 *);
    int (*eswitch_mode_get)(struct devlink *, u16 *);
    int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *);
    int (*eswitch_inline_mode_get)(struct devlink *, u8 *);
    int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *);
    int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *);
    int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *);
    int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *);
    int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *);
    int (*trap_init)(struct devlink *, const struct devlink_trap *, void *);
    void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *);
    int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action);
    int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>4.13</code> and <code>4.15</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*reload)(struct devlink *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_split)(struct devlink *, unsigned int, unsigned int)</code> ➡️ <code>int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_unsplit)(struct devlink *, unsigned int)</code> ➡️ <code>int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *)</code>
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
<code>int (*eswitch_mode_set)(struct devlink *, u16)</code> ➡️ <code>int (*eswitch_mode_set)(struct devlink *, u16, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*eswitch_inline_mode_set)(struct devlink *, u8)</code> ➡️ <code>int (*eswitch_inline_mode_set)(struct devlink *, u8, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*eswitch_encap_mode_set)(struct devlink *, u8)</code> ➡️ <code>int (*eswitch_encap_mode_set)(struct devlink *, u8, struct netlink_ext_ack *)</code>
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
<code>int (*info_get)(struct devlink *, struct devlink_info_req *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type)</code> ➡️ <code>int (*sb_pool_set)(struct devlink *, unsigned int, u16, u32, enum devlink_sb_threshold_type, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32)</code> ➡️ <code>int (*sb_port_pool_set)(struct devlink_port *, unsigned int, u16, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32)</code> ➡️ <code>int (*sb_tc_pool_bind_set)(struct devlink_port *, unsigned int, u16, enum devlink_sb_pool_type, u16, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*eswitch_encap_mode_get)(struct devlink *, u8 *)</code> ➡️ <code>int (*eswitch_encap_mode_get)(struct devlink *, enum devlink_eswitch_encap_mode *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*eswitch_encap_mode_set)(struct devlink *, u8, struct netlink_ext_ack *)</code> ➡️ <code>int (*eswitch_encap_mode_set)(struct devlink *, enum devlink_eswitch_encap_mode, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.3</code> and <code>5.4</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*reload_down)(struct devlink *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*reload_up)(struct devlink *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*trap_init)(struct devlink *, const struct devlink_trap *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*trap_fini)(struct devlink *, const struct devlink_trap *, void *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*trap_group_init)(struct devlink *, const struct devlink_trap_group *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*reload)(struct devlink *, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*trap_policer_init)(struct devlink *, const struct devlink_trap_policer *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*trap_policer_fini)(struct devlink *, const struct devlink_trap_policer *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*trap_policer_set)(struct devlink *, const struct devlink_trap_policer *, u64, u64, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*trap_policer_counter_get)(struct devlink *, const struct devlink_trap_policer *, u64 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*reload_down)(struct devlink *, struct netlink_ext_ack *)</code> ➡️ <code>int (*reload_down)(struct devlink *, bool, struct netlink_ext_ack *)</code>
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
<code>u32 supported_flash_update_params</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int reload_actions</code>
</li>
<li>
<b>Field added. </b>
<code>long unsigned int reload_limits</code>
</li>
<li>
<b>Field added. </b>
<code>int (*trap_group_action_set)(struct devlink *, const struct devlink_trap_group *, enum devlink_trap_action, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_function_hw_addr_get)(struct devlink *, struct devlink_port *, u8 *, int *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_function_hw_addr_set)(struct devlink *, struct devlink_port *, const u8 *, int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*reload_down)(struct devlink *, bool, struct netlink_ext_ack *)</code> ➡️ <code>int (*reload_down)(struct devlink *, bool, enum devlink_reload_action, enum devlink_reload_limit, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*reload_up)(struct devlink *, struct netlink_ext_ack *)</code> ➡️ <code>int (*reload_up)(struct devlink *, enum devlink_reload_action, enum devlink_reload_limit, u32 *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*flash_update)(struct devlink *, const char *, const char *, struct netlink_ext_ack *)</code> ➡️ <code>int (*flash_update)(struct devlink *, struct devlink_flash_update_params *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action)</code> ➡️ <code>int (*trap_action_set)(struct devlink *, const struct devlink_trap *, enum devlink_trap_action, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *)</code> ➡️ <code>int (*trap_group_set)(struct devlink *, const struct devlink_trap_group *, const struct devlink_trap_policer *, struct netlink_ext_ack *)</code>
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
<code>int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, unsigned int *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_del)(struct devlink *, unsigned int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_state_get)(struct devlink *, struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_state_set)(struct devlink *, struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *)</code>
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
<code>int (*trap_drop_counter_get)(struct devlink *, const struct devlink_trap *, u64 *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_leaf_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_leaf_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_node_tx_share_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_node_tx_max_set)(struct devlink_rate *, void *, u64, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_node_new)(struct devlink_rate *, void **, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_node_del)(struct devlink_rate *, void *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_leaf_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_node_parent_set)(struct devlink_rate *, struct devlink_rate *, void *, void *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_function_hw_addr_get)(struct devlink *, struct devlink_port *, u8 *, int *, struct netlink_ext_ack *)</code> ➡️ <code>int (*port_function_hw_addr_get)(struct devlink_port *, u8 *, int *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_function_hw_addr_set)(struct devlink *, struct devlink_port *, const u8 *, int, struct netlink_ext_ack *)</code> ➡️ <code>int (*port_function_hw_addr_set)(struct devlink_port *, const u8 *, int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_fn_state_get)(struct devlink *, struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *)</code> ➡️ <code>int (*port_fn_state_get)(struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_fn_state_set)(struct devlink *, struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *)</code> ➡️ <code>int (*port_fn_state_set)(struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>int (*port_split)(struct devlink *, unsigned int, unsigned int, struct netlink_ext_ack *)</code> ➡️ <code>int (*port_split)(struct devlink *, struct devlink_port *, unsigned int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_unsplit)(struct devlink *, unsigned int, struct netlink_ext_ack *)</code> ➡️ <code>int (*port_unsplit)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *)</code>
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
<code>int (*port_fn_roce_get)(struct devlink_port *, bool *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_roce_set)(struct devlink_port *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_migratable_get)(struct devlink_port *, bool *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*port_fn_migratable_set)(struct devlink_port *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_leaf_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_leaf_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_node_tx_priority_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*rate_node_tx_weight_set)(struct devlink_rate *, void *, u32, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>bool (*selftest_check)(struct devlink *, unsigned int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field added. </b>
<code>enum devlink_selftest_status (*selftest_run)(struct devlink *, unsigned int, struct netlink_ext_ack *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*port_type_set)(struct devlink_port *, enum devlink_port_type)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_split)(struct devlink *, struct devlink_port *, unsigned int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_unsplit)(struct devlink *, struct devlink_port *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_function_hw_addr_get)(struct devlink_port *, u8 *, int *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_function_hw_addr_set)(struct devlink_port *, const u8 *, int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_fn_roce_get)(struct devlink_port *, bool *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_fn_roce_set)(struct devlink_port *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_fn_migratable_get)(struct devlink_port *, bool *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_fn_migratable_set)(struct devlink_port *, bool, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_del)(struct devlink *, unsigned int, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_fn_state_get)(struct devlink_port *, enum devlink_port_fn_state *, enum devlink_port_fn_opstate *, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*port_fn_state_set)(struct devlink_port *, enum devlink_port_fn_state, struct netlink_ext_ack *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, unsigned int *)</code> ➡️ <code>int (*port_new)(struct devlink *, const struct devlink_port_new_attrs *, struct netlink_ext_ack *, struct devlink_port **)</code>
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
