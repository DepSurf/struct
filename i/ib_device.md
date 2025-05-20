# Struct: <code>ib_device</code>

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
In <code>4.13</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    char name[64];
    struct list_head event_handler_list;
    spinlock_t event_handler_lock;
    spinlock_t client_data_lock;
    struct list_head core_list;
    struct list_head client_data_list;
    struct ib_cache cache;
    struct ib_port_immutable *port_immutable;
    int num_comp_vectors;
    struct ib_port_pkey_list *port_pkey_list;
    struct iw_cm_verbs *iwcm;
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(struct ib_device *, u8, unsigned int, const union ib_gid *, const struct ib_gid_attr *, void **);
    int (*del_gid)(struct ib_device *, u8, unsigned int, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    struct ib_ucontext * (*alloc_ucontext)(struct ib_device *, struct ib_udata *);
    int (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    struct ib_pd * (*alloc_pd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *);
    struct ib_ah * (*create_ah)(struct ib_pd *, struct rdma_ah_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *);
    struct ib_srq * (*create_srq)(struct ib_pd *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *);
    int (*post_srq_recv)(struct ib_srq *, struct ib_recv_wr *, struct ib_recv_wr **);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *);
    int (*post_send)(struct ib_qp *, struct ib_send_wr *, struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, struct ib_recv_wr *, struct ib_recv_wr **);
    struct ib_cq * (*create_cq)(struct ib_device *, const struct ib_cq_init_attr *, struct ib_ucontext *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int);
    int (*destroy_flow)(struct ib_flow *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    struct module *owner;
    struct device dev;
    struct kobject *ports_parent;
    struct list_head port_list;
    enum (anon) reg_state;
    int uverbs_abi_ver;
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    struct uverbs_root_spec *specs_root;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    char name[64];
    struct list_head event_handler_list;
    spinlock_t event_handler_lock;
    spinlock_t client_data_lock;
    struct list_head core_list;
    struct list_head client_data_list;
    struct ib_cache cache;
    struct ib_port_immutable *port_immutable;
    int num_comp_vectors;
    struct ib_port_pkey_list *port_pkey_list;
    struct iw_cm_verbs *iwcm;
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const union ib_gid *, const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    struct ib_ucontext * (*alloc_ucontext)(struct ib_device *, struct ib_udata *);
    int (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    struct ib_pd * (*alloc_pd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *);
    struct ib_ah * (*create_ah)(struct ib_pd *, struct rdma_ah_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *);
    struct ib_srq * (*create_srq)(struct ib_pd *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *);
    int (*post_srq_recv)(struct ib_srq *, struct ib_recv_wr *, struct ib_recv_wr **);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *);
    int (*post_send)(struct ib_qp *, struct ib_send_wr *, struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, struct ib_recv_wr *, struct ib_recv_wr **);
    struct ib_cq * (*create_cq)(struct ib_device *, const struct ib_cq_init_attr *, struct ib_ucontext *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    struct module *owner;
    struct device dev;
    struct kobject *ports_parent;
    struct list_head port_list;
    enum (anon) reg_state;
    int uverbs_abi_ver;
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root res;
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    struct uverbs_root_spec *specs_root;
    enum rdma_driver_id driver_id;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct list_head event_handler_list;
    spinlock_t event_handler_lock;
    rwlock_t client_data_lock;
    struct list_head core_list;
    struct list_head client_data_list;
    struct ib_cache cache;
    struct ib_port_immutable *port_immutable;
    int num_comp_vectors;
    struct ib_port_pkey_list *port_pkey_list;
    struct iw_cm_verbs *iwcm;
    struct module *owner;
    struct device dev;
    const struct attribute_group * groups[3];
    struct kobject *ports_kobj;
    struct list_head port_list;
    enum (anon) reg_state;
    int uverbs_abi_ver;
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root res;
    const struct uapi_definition *driver_def;
    enum rdma_driver_id driver_id;
    refcount_t refcount;
    struct completion unreg_completion;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u32 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[4];
    u64 uverbs_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u32 phys_port_cnt;
    struct ib_device_attr attrs;
    struct hw_stats_device_data *hw_stats_data;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[4];
    u64 uverbs_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u32 phys_port_cnt;
    struct ib_device_attr attrs;
    struct hw_stats_device_data *hw_stats_data;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[4];
    u64 uverbs_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u32 phys_port_cnt;
    struct ib_device_attr attrs;
    struct hw_stats_device_data *hw_stats_data;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[4];
    u64 uverbs_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u32 phys_port_cnt;
    struct ib_device_attr attrs;
    struct hw_stats_device_data *hw_stats_data;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t qp_open_list_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    rwlock_t cache_lock;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[4];
    u64 uverbs_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u32 phys_port_cnt;
    struct ib_device_attr attrs;
    struct hw_stats_device_data *hw_stats_data;
    struct rdmacg_device cg_device;
    u32 index;
    spinlock_t cq_pools_lock;
    struct list_head cq_pools[3];
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
    u32 lag_flags;
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
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
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
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ib_device {
    struct device *dma_device;
    struct ib_device_ops ops;
    char name[64];
    struct callback_head callback_head;
    struct list_head event_handler_list;
    struct rw_semaphore event_handler_rwsem;
    spinlock_t event_handler_lock;
    struct rw_semaphore client_data_rwsem;
    struct xarray client_data;
    struct mutex unregistration_lock;
    struct ib_cache cache;
    struct ib_port_data *port_data;
    int num_comp_vectors;
    struct device dev;
    struct ib_core_device coredev;
    const struct attribute_group * groups[3];
    u64 uverbs_cmd_mask;
    u64 uverbs_ex_cmd_mask;
    char node_desc[64];
    __be64 node_guid;
    u32 local_dma_lkey;
    u16 is_switch;
    u16 kverbs_provider;
    u16 use_cq_dim;
    u8 node_type;
    u8 phys_port_cnt;
    struct ib_device_attr attrs;
    struct attribute_group *hw_stats_ag;
    struct rdma_hw_stats *hw_stats;
    struct rdmacg_device cg_device;
    u32 index;
    struct rdma_restrack_root *res;
    const struct uapi_definition *driver_def;
    refcount_t refcount;
    struct completion unreg_completion;
    struct work_struct unregistration_work;
    const struct rdma_link_ops *link_ops;
    struct mutex compat_devs_mutex;
    struct xarray compat_devs;
    char iw_ifname[16];
    u32 iw_driver_flags;
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
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*destroy_flow_action)(struct ib_flow_action *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dealloc_dm)(struct ib_dm *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*destroy_counters)(struct ib_counters *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct rdma_restrack_root res</code>
</li>
<li>
<b>Field added. </b>
<code>enum rdma_driver_id driver_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*add_gid)(struct ib_device *, u8, unsigned int, const union ib_gid *, const struct ib_gid_attr *, void **)</code> ➡️ <code>int (*add_gid)(const union ib_gid *, const struct ib_gid_attr *, void **)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*del_gid)(struct ib_device *, u8, unsigned int, void **)</code> ➡️ <code>int (*del_gid)(const struct ib_gid_attr *, void **)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int)</code> ➡️ <code>struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *)</code>
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
<code>struct ib_device_ops ops</code>
</li>
<li>
<b>Field added. </b>
<code>const struct attribute_group * groups[3]</code>
</li>
<li>
<b>Field added. </b>
<code>struct kobject *ports_kobj</code>
</li>
<li>
<b>Field added. </b>
<code>const struct uapi_definition *driver_def</code>
</li>
<li>
<b>Field added. </b>
<code>refcount_t refcount</code>
</li>
<li>
<b>Field added. </b>
<code>struct completion unreg_completion</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_port)(struct ib_device *, u8, struct ib_port_attr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct net_device * (*get_netdev)(struct ib_device *, u8)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_gid)(struct ib_device *, u8, int, union ib_gid *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*add_gid)(const union ib_gid *, const struct ib_gid_attr *, void **)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*del_gid)(const struct ib_gid_attr *, void **)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_pkey)(struct ib_device *, u8, u16, u16 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_device)(struct ib_device *, int, struct ib_device_modify *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_ucontext * (*alloc_ucontext)(struct ib_device *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dealloc_ucontext)(struct ib_ucontext *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*mmap)(struct ib_ucontext *, struct vm_area_struct *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_pd * (*alloc_pd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dealloc_pd)(struct ib_pd *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_ah * (*create_ah)(struct ib_pd *, struct rdma_ah_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_ah)(struct ib_ah *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_srq * (*create_srq)(struct ib_pd *, struct ib_srq_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_srq)(struct ib_srq *, struct ib_srq_attr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_srq)(struct ib_srq *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*post_srq_recv)(struct ib_srq *, struct ib_recv_wr *, struct ib_recv_wr **)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_qp)(struct ib_qp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*post_send)(struct ib_qp *, struct ib_send_wr *, struct ib_send_wr **)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*post_recv)(struct ib_qp *, struct ib_recv_wr *, struct ib_recv_wr **)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_cq * (*create_cq)(struct ib_device *, const struct ib_cq_init_attr *, struct ib_ucontext *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_cq)(struct ib_cq *, u16, u16)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_cq)(struct ib_cq *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*resize_cq)(struct ib_cq *, int, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*poll_cq)(struct ib_cq *, int, struct ib_wc *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*peek_cq)(struct ib_cq *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*req_ncomp_notif)(struct ib_cq *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_mr * (*get_dma_mr)(struct ib_pd *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dereg_mr)(struct ib_mr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dealloc_mw)(struct ib_mw *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*unmap_fmr)(struct list_head *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dealloc_fmr)(struct ib_fmr *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dealloc_xrcd)(struct ib_xrcd *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_flow)(struct ib_flow *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*disassociate_ucontext)(struct ib_ucontext *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*drain_rq)(struct ib_qp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*drain_sq)(struct ib_qp *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_vf_link_state)(struct ib_device *, int, u8, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*set_vf_guid)(struct ib_device *, int, u8, u64, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_wq)(struct ib_wq *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_flow_action)(struct ib_flow_action *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*dealloc_dm)(struct ib_dm *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*destroy_counters)(struct ib_counters *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *))</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kobject *ports_parent</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *)</code>
</li>
<li>
<b>Field removed. </b>
<code>void (*get_dev_fw_str)(struct ib_device *, char *)</code>
</li>
<li>
<b>Field removed. </b>
<code>const struct cpumask * (*get_vector_affinity)(struct ib_device *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct uverbs_root_spec *specs_root</code>
</li>
<li>
<b>Field type changed. </b>
<code>spinlock_t client_data_lock</code> ➡️ <code>rwlock_t client_data_lock</code>
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
<code>struct callback_head callback_head</code>
</li>
<li>
<b>Field added. </b>
<code>struct rw_semaphore client_data_rwsem</code>
</li>
<li>
<b>Field added. </b>
<code>struct xarray client_data</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex unregistration_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct ib_port_data *port_data</code>
</li>
<li>
<b>Field added. </b>
<code>struct ib_core_device coredev</code>
</li>
<li>
<b>Field added. </b>
<code>u16 kverbs_provider</code>
</li>
<li>
<b>Field added. </b>
<code>u16 use_cq_dim</code>
</li>
<li>
<b>Field added. </b>
<code>struct work_struct unregistration_work</code>
</li>
<li>
<b>Field added. </b>
<code>const struct rdma_link_ops *link_ops</code>
</li>
<li>
<b>Field added. </b>
<code>struct mutex compat_devs_mutex</code>
</li>
<li>
<b>Field added. </b>
<code>struct xarray compat_devs</code>
</li>
<li>
<b>Field added. </b>
<code>char iw_ifname[16]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 iw_driver_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>rwlock_t client_data_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head core_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head client_data_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_port_immutable *port_immutable</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_port_pkey_list *port_pkey_list</code>
</li>
<li>
<b>Field removed. </b>
<code>struct iw_cm_verbs *iwcm</code>
</li>
<li>
<b>Field removed. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field removed. </b>
<code>struct kobject *ports_kobj</code>
</li>
<li>
<b>Field removed. </b>
<code>struct list_head port_list</code>
</li>
<li>
<b>Field removed. </b>
<code>enum (anon) reg_state</code>
</li>
<li>
<b>Field removed. </b>
<code>int uverbs_abi_ver</code>
</li>
<li>
<b>Field removed. </b>
<code>enum rdma_driver_id driver_id</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rdma_restrack_root res</code> ➡️ <code>struct rdma_restrack_root *res</code>
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
<code>struct rw_semaphore event_handler_rwsem</code>
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
<code>spinlock_t qp_open_list_lock</code>
</li>
<li>
<b>Field added. </b>
<code>rwlock_t cache_lock</code>
</li>
<li>
<b>Field added. </b>
<code>spinlock_t cq_pools_lock</code>
</li>
<li>
<b>Field added. </b>
<code>struct list_head cq_pools[3]</code>
</li>
<li>
<b>Field added. </b>
<code>u32 lag_flags</code>
</li>
<li>
<b>Field removed. </b>
<code>spinlock_t event_handler_lock</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_cache cache</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>u64 uverbs_ex_cmd_mask</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>u8 phys_port_cnt</code> ➡️ <code>u32 phys_port_cnt</code>
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
<code>struct hw_stats_device_data *hw_stats_data</code>
</li>
<li>
<b>Field removed. </b>
<code>struct attribute_group *hw_stats_ag</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rdma_hw_stats *hw_stats</code>
</li>
<li>
<b>Field type changed. </b>
<code>const struct attribute_group * groups[3]</code> ➡️ <code>const struct attribute_group * groups[4]</code>
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
