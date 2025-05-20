# Struct: <code>ib_device_ops</code>

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
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ib_device_ops {
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    struct ib_ucontext * (*alloc_ucontext)(struct ib_device *, struct ib_udata *);
    int (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    struct ib_pd * (*alloc_pd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *);
    struct ib_ah * (*create_ah)(struct ib_pd *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    struct ib_srq * (*create_srq)(struct ib_pd *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *);
    struct ib_cq * (*create_cq)(struct ib_device *, const struct ib_cq_init_attr *, struct ib_ucontext *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u8, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    int (*alloc_mw)(struct ib_mw *, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u8, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *);
    size_t size_ib_ah;
    size_t size_ib_counters;
    size_t size_ib_cq;
    size_t size_ib_mw;
    size_t size_ib_pd;
    size_t size_ib_rwq_ind_table;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
    size_t size_ib_xrcd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u32, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u32, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u32, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u32, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u32);
    struct net_device * (*get_netdev)(struct ib_device *, u32);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u32, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u32, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u32, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u32, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    struct ib_mr * (*reg_user_mr_dmabuf)(struct ib_pd *, u64, u64, u64, int, int, struct ib_udata *);
    struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    int (*alloc_mw)(struct ib_mw *, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u32, int);
    int (*get_vf_config)(struct ib_device *, int, u32, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u32, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u32, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u32, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u32);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u32, int);
    int (*init_port)(struct ib_device *, u32, struct kobject *);
    int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *);
    size_t size_ib_ah;
    size_t size_ib_counters;
    size_t size_ib_cq;
    size_t size_ib_mw;
    size_t size_ib_pd;
    size_t size_ib_rwq_ind_table;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
    size_t size_ib_xrcd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    const struct attribute_group *device_group;
    const struct attribute_group **port_groups;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u32, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u32, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u32, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u32, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u32);
    struct net_device * (*get_netdev)(struct ib_device *, u32);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u32, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u32, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u32, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u32, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    int (*create_qp)(struct ib_qp *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    struct ib_mr * (*reg_user_mr_dmabuf)(struct ib_pd *, u64, u64, u64, int, int, struct ib_udata *);
    struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    int (*alloc_mw)(struct ib_mw *, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u32, int);
    int (*get_vf_config)(struct ib_device *, int, u32, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u32, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u32, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u32, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_device_stats)(struct ib_device *);
    struct rdma_hw_stats * (*alloc_hw_port_stats)(struct ib_device *, u32);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u32, int);
    int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *);
    int (*get_numa_node)(struct ib_device *);
    size_t size_ib_ah;
    size_t size_ib_counters;
    size_t size_ib_cq;
    size_t size_ib_mw;
    size_t size_ib_pd;
    size_t size_ib_qp;
    size_t size_ib_rwq_ind_table;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
    size_t size_ib_xrcd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    const struct attribute_group *device_group;
    const struct attribute_group **port_groups;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u32, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u32, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u32, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u32, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u32);
    struct net_device * (*get_netdev)(struct ib_device *, u32);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u32, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u32, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u32, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u32, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    int (*create_qp)(struct ib_qp *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    struct ib_mr * (*reg_user_mr_dmabuf)(struct ib_pd *, u64, u64, u64, int, int, struct ib_udata *);
    struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    int (*alloc_mw)(struct ib_mw *, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*set_vf_link_state)(struct ib_device *, int, u32, int);
    int (*get_vf_config)(struct ib_device *, int, u32, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u32, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u32, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u32, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_device_stats)(struct ib_device *);
    struct rdma_hw_stats * (*alloc_hw_port_stats)(struct ib_device *, u32);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u32, int);
    int (*modify_hw_stat)(struct ib_device *, u32, unsigned int, bool);
    int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *);
    int (*get_numa_node)(struct ib_device *);
    size_t size_ib_ah;
    size_t size_ib_counters;
    size_t size_ib_cq;
    size_t size_ib_mw;
    size_t size_ib_pd;
    size_t size_ib_qp;
    size_t size_ib_rwq_ind_table;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
    size_t size_ib_xrcd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    const struct attribute_group *device_group;
    const struct attribute_group **port_groups;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u32, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u32, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u32, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u32, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u32);
    struct net_device * (*get_netdev)(struct ib_device *, u32);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u32, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u32, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u32, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u32, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    int (*create_qp)(struct ib_qp *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    struct ib_mr * (*reg_user_mr_dmabuf)(struct ib_pd *, u64, u64, u64, int, int, struct ib_udata *);
    struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    int (*alloc_mw)(struct ib_mw *, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*set_vf_link_state)(struct ib_device *, int, u32, int);
    int (*get_vf_config)(struct ib_device *, int, u32, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u32, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u32, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u32, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_device_stats)(struct ib_device *);
    struct rdma_hw_stats * (*alloc_hw_port_stats)(struct ib_device *, u32);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u32, int);
    int (*modify_hw_stat)(struct ib_device *, u32, unsigned int, bool);
    int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *);
    int (*get_numa_node)(struct ib_device *);
    size_t size_ib_ah;
    size_t size_ib_counters;
    size_t size_ib_cq;
    size_t size_ib_mw;
    size_t size_ib_pd;
    size_t size_ib_qp;
    size_t size_ib_rwq_ind_table;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
    size_t size_ib_xrcd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    const struct attribute_group *device_group;
    const struct attribute_group **port_groups;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u32, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u32, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u32, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u32, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u32);
    struct net_device * (*get_netdev)(struct ib_device *, u32);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u32, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u32, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u32, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u32, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    int (*create_qp)(struct ib_qp *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    struct ib_mr * (*reg_user_mr_dmabuf)(struct ib_pd *, u64, u64, u64, int, int, struct ib_udata *);
    struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    int (*alloc_mw)(struct ib_mw *, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*set_vf_link_state)(struct ib_device *, int, u32, int);
    int (*get_vf_config)(struct ib_device *, int, u32, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u32, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u32, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u32, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_device_stats)(struct ib_device *);
    struct rdma_hw_stats * (*alloc_hw_port_stats)(struct ib_device *, u32);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u32, int);
    int (*modify_hw_stat)(struct ib_device *, u32, unsigned int, bool);
    int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *);
    int (*get_numa_node)(struct ib_device *);
    size_t size_ib_ah;
    size_t size_ib_counters;
    size_t size_ib_cq;
    size_t size_ib_mw;
    size_t size_ib_pd;
    size_t size_ib_qp;
    size_t size_ib_rwq_ind_table;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
    size_t size_ib_xrcd;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    const struct attribute_group *device_group;
    const struct attribute_group **port_groups;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u32, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u32, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u32, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u32, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u32);
    struct net_device * (*get_netdev)(struct ib_device *, u32);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u32, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u32, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u32, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u32, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    int (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    int (*create_qp)(struct ib_qp *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    int (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    struct ib_mr * (*reg_user_mr_dmabuf)(struct ib_pd *, u64, u64, u64, int, int, struct ib_udata *);
    struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    int (*alloc_mw)(struct ib_mw *, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*set_vf_link_state)(struct ib_device *, int, u32, int);
    int (*get_vf_config)(struct ib_device *, int, u32, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u32, struct ifla_vf_stats *);
    int (*get_vf_guid)(struct ib_device *, int, u32, struct ifla_vf_guid *, struct ifla_vf_guid *);
    int (*set_vf_guid)(struct ib_device *, int, u32, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    int (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_device_stats)(struct ib_device *);
    struct rdma_hw_stats * (*alloc_hw_port_stats)(struct ib_device *, u32);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u32, int);
    int (*modify_hw_stat)(struct ib_device *, u32, unsigned int, bool);
    int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *);
    int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *);
    int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *);
    int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *);
    int (*fill_res_srq_entry)(struct sk_buff *, struct ib_srq *);
    int (*fill_res_srq_entry_raw)(struct sk_buff *, struct ib_srq *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *);
    int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *);
    int (*get_numa_node)(struct ib_device *);
    size_t size_ib_ah;
    size_t size_ib_counters;
    size_t size_ib_cq;
    size_t size_ib_mw;
    size_t size_ib_pd;
    size_t size_ib_qp;
    size_t size_ib_rwq_ind_table;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
    size_t size_ib_xrcd;
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
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
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
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ib_device_ops {
    struct module *owner;
    enum rdma_driver_id driver_id;
    u32 uverbs_abi_ver;
    unsigned int uverbs_no_driver_id_binding;
    int (*post_send)(struct ib_qp *, const struct ib_send_wr *, const struct ib_send_wr **);
    int (*post_recv)(struct ib_qp *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    void (*drain_rq)(struct ib_qp *);
    void (*drain_sq)(struct ib_qp *);
    int (*poll_cq)(struct ib_cq *, int, struct ib_wc *);
    int (*peek_cq)(struct ib_cq *, int);
    int (*req_notify_cq)(struct ib_cq *, enum ib_cq_notify_flags);
    int (*req_ncomp_notif)(struct ib_cq *, int);
    int (*post_srq_recv)(struct ib_srq *, const struct ib_recv_wr *, const struct ib_recv_wr **);
    int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *);
    int (*query_device)(struct ib_device *, struct ib_device_attr *, struct ib_udata *);
    int (*modify_device)(struct ib_device *, int, struct ib_device_modify *);
    void (*get_dev_fw_str)(struct ib_device *, char *);
    const struct cpumask * (*get_vector_affinity)(struct ib_device *, int);
    int (*query_port)(struct ib_device *, u8, struct ib_port_attr *);
    int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *);
    int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *);
    enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8);
    struct net_device * (*get_netdev)(struct ib_device *, u8);
    struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *));
    int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *);
    int (*query_gid)(struct ib_device *, u8, int, union ib_gid *);
    int (*add_gid)(const struct ib_gid_attr *, void **);
    int (*del_gid)(const struct ib_gid_attr *, void **);
    int (*query_pkey)(struct ib_device *, u8, u16, u16 *);
    int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *);
    void (*dealloc_ucontext)(struct ib_ucontext *);
    int (*mmap)(struct ib_ucontext *, struct vm_area_struct *);
    void (*mmap_free)(struct rdma_user_mmap_entry *);
    void (*disassociate_ucontext)(struct ib_ucontext *);
    int (*alloc_pd)(struct ib_pd *, struct ib_udata *);
    void (*dealloc_pd)(struct ib_pd *, struct ib_udata *);
    int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *);
    int (*modify_ah)(struct ib_ah *, struct rdma_ah_attr *);
    int (*query_ah)(struct ib_ah *, struct rdma_ah_attr *);
    void (*destroy_ah)(struct ib_ah *, u32);
    int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *);
    int (*modify_srq)(struct ib_srq *, struct ib_srq_attr *, enum ib_srq_attr_mask, struct ib_udata *);
    int (*query_srq)(struct ib_srq *, struct ib_srq_attr *);
    void (*destroy_srq)(struct ib_srq *, struct ib_udata *);
    struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *);
    int (*modify_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_udata *);
    int (*query_qp)(struct ib_qp *, struct ib_qp_attr *, int, struct ib_qp_init_attr *);
    int (*destroy_qp)(struct ib_qp *, struct ib_udata *);
    int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *);
    int (*modify_cq)(struct ib_cq *, u16, u16);
    void (*destroy_cq)(struct ib_cq *, struct ib_udata *);
    int (*resize_cq)(struct ib_cq *, int, struct ib_udata *);
    struct ib_mr * (*get_dma_mr)(struct ib_pd *, int);
    struct ib_mr * (*reg_user_mr)(struct ib_pd *, u64, u64, u64, int, struct ib_udata *);
    int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *);
    int (*dereg_mr)(struct ib_mr *, struct ib_udata *);
    struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *);
    struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32);
    int (*advise_mr)(struct ib_pd *, enum ib_uverbs_advise_mr_advice, u32, struct ib_sge *, u32, struct uverbs_attr_bundle *);
    int (*map_mr_sg)(struct ib_mr *, struct scatterlist *, int, unsigned int *);
    int (*check_mr_status)(struct ib_mr *, u32, struct ib_mr_status *);
    struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *);
    int (*dealloc_mw)(struct ib_mw *);
    struct ib_fmr * (*alloc_fmr)(struct ib_pd *, int, struct ib_fmr_attr *);
    int (*map_phys_fmr)(struct ib_fmr *, u64 *, int, u64);
    int (*unmap_fmr)(struct list_head *);
    int (*dealloc_fmr)(struct ib_fmr *);
    void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int);
    int (*attach_mcast)(struct ib_qp *, union ib_gid *, u16);
    int (*detach_mcast)(struct ib_qp *, union ib_gid *, u16);
    struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *);
    int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *);
    struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *);
    int (*destroy_flow)(struct ib_flow *);
    struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*destroy_flow_action)(struct ib_flow_action *);
    int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *);
    int (*set_vf_link_state)(struct ib_device *, int, u8, int);
    int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *);
    int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *);
    int (*set_vf_guid)(struct ib_device *, int, u8, u64, int);
    struct ib_wq * (*create_wq)(struct ib_pd *, struct ib_wq_init_attr *, struct ib_udata *);
    void (*destroy_wq)(struct ib_wq *, struct ib_udata *);
    int (*modify_wq)(struct ib_wq *, struct ib_wq_attr *, u32, struct ib_udata *);
    struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *);
    int (*destroy_rwq_ind_table)(struct ib_rwq_ind_table *);
    struct ib_dm * (*alloc_dm)(struct ib_device *, struct ib_ucontext *, struct ib_dm_alloc_attr *, struct uverbs_attr_bundle *);
    int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *);
    struct ib_mr * (*reg_dm_mr)(struct ib_pd *, struct ib_dm *, struct ib_dm_mr_attr *, struct uverbs_attr_bundle *);
    struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *);
    int (*destroy_counters)(struct ib_counters *);
    int (*read_counters)(struct ib_counters *, struct ib_counters_read_attr *, struct uverbs_attr_bundle *);
    int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *);
    struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8);
    int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int);
    int (*init_port)(struct ib_device *, u8, struct kobject *);
    int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *);
    int (*enable_driver)(struct ib_device *);
    void (*dealloc_driver)(struct ib_device *);
    void (*iw_add_ref)(struct ib_qp *);
    void (*iw_rem_ref)(struct ib_qp *);
    struct ib_qp * (*iw_get_qp)(struct ib_device *, int);
    int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *);
    int (*iw_reject)(struct iw_cm_id *, const void *, u8);
    int (*iw_create_listen)(struct iw_cm_id *, int);
    int (*iw_destroy_listen)(struct iw_cm_id *);
    int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *);
    int (*counter_unbind_qp)(struct ib_qp *);
    int (*counter_dealloc)(struct rdma_counter *);
    struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *);
    int (*counter_update_stats)(struct rdma_counter *);
    size_t size_ib_ah;
    size_t size_ib_cq;
    size_t size_ib_pd;
    size_t size_ib_srq;
    size_t size_ib_ucontext;
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
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct module *owner</code>
</li>
<li>
<b>Field added. </b>
<code>enum rdma_driver_id driver_id</code>
</li>
<li>
<b>Field added. </b>
<code>u32 uverbs_abi_ver</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int uverbs_no_driver_id_binding</code>
</li>
<li>
<b>Field added. </b>
<code>struct ib_mr * (*alloc_mr_integrity)(struct ib_pd *, u32, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*map_mr_sg_pi)(struct ib_mr *, struct scatterlist *, int, unsigned int *, struct scatterlist *, int, unsigned int *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*init_port)(struct ib_device *, u8, struct kobject *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*enable_driver)(struct ib_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*dealloc_driver)(struct ib_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*iw_add_ref)(struct ib_qp *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*iw_rem_ref)(struct ib_qp *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct ib_qp * (*iw_get_qp)(struct ib_device *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*iw_connect)(struct iw_cm_id *, struct iw_cm_conn_param *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*iw_accept)(struct iw_cm_id *, struct iw_cm_conn_param *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*iw_reject)(struct iw_cm_id *, const void *, u8)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*iw_create_listen)(struct iw_cm_id *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*iw_destroy_listen)(struct iw_cm_id *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*counter_bind_qp)(struct rdma_counter *, struct ib_qp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*counter_unbind_qp)(struct ib_qp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*counter_dealloc)(struct rdma_counter *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct rdma_hw_stats * (*counter_alloc_stats)(struct rdma_counter *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*counter_update_stats)(struct rdma_counter *)</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_ah</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_cq</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_pd</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_srq</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_ucontext</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_ucontext * (*alloc_ucontext)(struct ib_device *, struct ib_udata *)</code> ➡️ <code>int (*alloc_ucontext)(struct ib_ucontext *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dealloc_ucontext)(struct ib_ucontext *)</code> ➡️ <code>void (*dealloc_ucontext)(struct ib_ucontext *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_pd * (*alloc_pd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *)</code> ➡️ <code>int (*alloc_pd)(struct ib_pd *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dealloc_pd)(struct ib_pd *)</code> ➡️ <code>void (*dealloc_pd)(struct ib_pd *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_ah * (*create_ah)(struct ib_pd *, struct rdma_ah_attr *, u32, struct ib_udata *)</code> ➡️ <code>int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*destroy_ah)(struct ib_ah *, u32)</code> ➡️ <code>void (*destroy_ah)(struct ib_ah *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_srq * (*create_srq)(struct ib_pd *, struct ib_srq_init_attr *, struct ib_udata *)</code> ➡️ <code>int (*create_srq)(struct ib_srq *, struct ib_srq_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*destroy_srq)(struct ib_srq *)</code> ➡️ <code>void (*destroy_srq)(struct ib_srq *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*destroy_qp)(struct ib_qp *)</code> ➡️ <code>int (*destroy_qp)(struct ib_qp *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_cq * (*create_cq)(struct ib_device *, const struct ib_cq_init_attr *, struct ib_ucontext *, struct ib_udata *)</code> ➡️ <code>int (*create_cq)(struct ib_cq *, const struct ib_cq_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*destroy_cq)(struct ib_cq *)</code> ➡️ <code>void (*destroy_cq)(struct ib_cq *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dereg_mr)(struct ib_mr *)</code> ➡️ <code>int (*dereg_mr)(struct ib_mr *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32)</code> ➡️ <code>struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_ucontext *, struct ib_udata *)</code> ➡️ <code>struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dealloc_xrcd)(struct ib_xrcd *)</code> ➡️ <code>int (*dealloc_xrcd)(struct ib_xrcd *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*destroy_wq)(struct ib_wq *)</code> ➡️ <code>void (*destroy_wq)(struct ib_wq *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*dealloc_dm)(struct ib_dm *)</code> ➡️ <code>int (*dealloc_dm)(struct ib_dm *, struct uverbs_attr_bundle *)</code>
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
<code>void (*mmap_free)(struct rdma_user_mmap_entry *)</code>
</li>
<li>
<b>Field added. </b>
<code>void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int)</code>
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
<code>int (*get_vf_guid)(struct ib_device *, int, u8, struct ifla_vf_guid *, struct ifla_vf_guid *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_stat_entry)(struct sk_buff *, struct rdma_restrack_entry *)</code>
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
<code>void (*invalidate_range)(struct ib_umem_odp *, long unsigned int, long unsigned int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad_hdr *, size_t, struct ib_mad_hdr *, size_t *, u16 *)</code> ➡️ <code>int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*create_ah)(struct ib_ah *, struct rdma_ah_attr *, u32, struct ib_udata *)</code> ➡️ <code>int (*create_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *)</code>
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
<code>int (*create_user_ah)(struct ib_ah *, struct rdma_ah_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_mr_entry)(struct sk_buff *, struct ib_mr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_mr_entry_raw)(struct sk_buff *, struct ib_mr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_cq_entry)(struct sk_buff *, struct ib_cq *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_cq_entry_raw)(struct sk_buff *, struct ib_cq *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_qp_entry)(struct sk_buff *, struct ib_qp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_qp_entry_raw)(struct sk_buff *, struct ib_qp *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_cm_id_entry)(struct sk_buff *, struct rdma_cm_id *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_stat_mr_entry)(struct sk_buff *, struct ib_mr *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*query_ucontext)(struct ib_ucontext *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_counters</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_mw</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_rwq_ind_table</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_xrcd</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*fill_res_entry)(struct sk_buff *, struct rdma_restrack_entry *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*fill_stat_entry)(struct sk_buff *, struct rdma_restrack_entry *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*dealloc_pd)(struct ib_pd *, struct ib_udata *)</code> ➡️ <code>int (*dealloc_pd)(struct ib_pd *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*destroy_ah)(struct ib_ah *, u32)</code> ➡️ <code>int (*destroy_ah)(struct ib_ah *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*destroy_srq)(struct ib_srq *, struct ib_udata *)</code> ➡️ <code>int (*destroy_srq)(struct ib_srq *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*destroy_cq)(struct ib_cq *, struct ib_udata *)</code> ➡️ <code>int (*destroy_cq)(struct ib_cq *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *)</code> ➡️ <code>struct ib_mr * (*rereg_user_mr)(struct ib_mr *, int, u64, u64, u64, int, struct ib_pd *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32, struct ib_udata *)</code> ➡️ <code>struct ib_mr * (*alloc_mr)(struct ib_pd *, enum ib_mr_type, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_mw * (*alloc_mw)(struct ib_pd *, enum ib_mw_type, struct ib_udata *)</code> ➡️ <code>int (*alloc_mw)(struct ib_mw *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_xrcd * (*alloc_xrcd)(struct ib_device *, struct ib_udata *)</code> ➡️ <code>int (*alloc_xrcd)(struct ib_xrcd *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, int, struct ib_udata *)</code> ➡️ <code>struct ib_flow * (*create_flow)(struct ib_qp *, struct ib_flow_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>void (*destroy_wq)(struct ib_wq *, struct ib_udata *)</code> ➡️ <code>int (*destroy_wq)(struct ib_wq *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_rwq_ind_table * (*create_rwq_ind_table)(struct ib_device *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *)</code> ➡️ <code>int (*create_rwq_ind_table)(struct ib_rwq_ind_table *, struct ib_rwq_ind_table_init_attr *, struct ib_udata *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_counters * (*create_counters)(struct ib_device *, struct uverbs_attr_bundle *)</code> ➡️ <code>int (*create_counters)(struct ib_counters *, struct uverbs_attr_bundle *)</code>
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
<code>struct ib_mr * (*reg_user_mr_dmabuf)(struct ib_pd *, u64, u64, u64, int, int, struct ib_udata *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*req_ncomp_notif)(struct ib_cq *, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*process_mad)(struct ib_device *, int, u8, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *)</code> ➡️ <code>int (*process_mad)(struct ib_device *, int, u32, const struct ib_wc *, const struct ib_grh *, const struct ib_mad *, struct ib_mad *, size_t *, u16 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*query_port)(struct ib_device *, u8, struct ib_port_attr *)</code> ➡️ <code>int (*query_port)(struct ib_device *, u32, struct ib_port_attr *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*modify_port)(struct ib_device *, u8, int, struct ib_port_modify *)</code> ➡️ <code>int (*modify_port)(struct ib_device *, u32, int, struct ib_port_modify *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_port_immutable)(struct ib_device *, u8, struct ib_port_immutable *)</code> ➡️ <code>int (*get_port_immutable)(struct ib_device *, u32, struct ib_port_immutable *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>enum rdma_link_layer (*get_link_layer)(struct ib_device *, u8)</code> ➡️ <code>enum rdma_link_layer (*get_link_layer)(struct ib_device *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct net_device * (*get_netdev)(struct ib_device *, u8)</code> ➡️ <code>struct net_device * (*get_netdev)(struct ib_device *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u8, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *))</code> ➡️ <code>struct net_device * (*alloc_rdma_netdev)(struct ib_device *, u32, enum rdma_netdev_t, const char *, unsigned char, void(*)(struct net_device *))</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*rdma_netdev_get_params)(struct ib_device *, u8, enum rdma_netdev_t, struct rdma_netdev_alloc_params *)</code> ➡️ <code>int (*rdma_netdev_get_params)(struct ib_device *, u32, enum rdma_netdev_t, struct rdma_netdev_alloc_params *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*query_gid)(struct ib_device *, u8, int, union ib_gid *)</code> ➡️ <code>int (*query_gid)(struct ib_device *, u32, int, union ib_gid *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*query_pkey)(struct ib_device *, u8, u16, u16 *)</code> ➡️ <code>int (*query_pkey)(struct ib_device *, u32, u16, u16 *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_vf_link_state)(struct ib_device *, int, u8, int)</code> ➡️ <code>int (*set_vf_link_state)(struct ib_device *, int, u32, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_vf_config)(struct ib_device *, int, u8, struct ifla_vf_info *)</code> ➡️ <code>int (*get_vf_config)(struct ib_device *, int, u32, struct ifla_vf_info *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_vf_stats)(struct ib_device *, int, u8, struct ifla_vf_stats *)</code> ➡️ <code>int (*get_vf_stats)(struct ib_device *, int, u32, struct ifla_vf_stats *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_vf_guid)(struct ib_device *, int, u8, struct ifla_vf_guid *, struct ifla_vf_guid *)</code> ➡️ <code>int (*get_vf_guid)(struct ib_device *, int, u32, struct ifla_vf_guid *, struct ifla_vf_guid *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*set_vf_guid)(struct ib_device *, int, u8, u64, int)</code> ➡️ <code>int (*set_vf_guid)(struct ib_device *, int, u32, u64, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u8)</code> ➡️ <code>struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u32)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u8, int)</code> ➡️ <code>int (*get_hw_stats)(struct ib_device *, struct rdma_hw_stats *, u32, int)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*init_port)(struct ib_device *, u8, struct kobject *)</code> ➡️ <code>int (*init_port)(struct ib_device *, u32, struct kobject *)</code>
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
<code>const struct attribute_group *device_group</code>
</li>
<li>
<b>Field added. </b>
<code>const struct attribute_group **port_groups</code>
</li>
<li>
<b>Field added. </b>
<code>struct rdma_hw_stats * (*alloc_hw_device_stats)(struct ib_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>struct rdma_hw_stats * (*alloc_hw_port_stats)(struct ib_device *, u32)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*get_numa_node)(struct ib_device *)</code>
</li>
<li>
<b>Field added. </b>
<code>size_t size_ib_qp</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rdma_hw_stats * (*alloc_hw_stats)(struct ib_device *, u32)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*init_port)(struct ib_device *, u32, struct kobject *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct ib_qp * (*create_qp)(struct ib_pd *, struct ib_qp_init_attr *, struct ib_udata *)</code> ➡️ <code>int (*create_qp)(struct ib_qp *, struct ib_qp_init_attr *, struct ib_udata *)</code>
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
<code>int (*modify_hw_stat)(struct ib_device *, u32, unsigned int, bool)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct ib_flow_action * (*create_flow_action_esp)(struct ib_device *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *)</code>
</li>
<li>
<b>Field removed. </b>
<code>int (*modify_flow_action_esp)(struct ib_flow_action *, const struct ib_flow_action_attrs_esp *, struct uverbs_attr_bundle *)</code>
</li>
</ul>
</details>
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
<b>Field added. </b>
<code>int (*fill_res_srq_entry)(struct sk_buff *, struct ib_srq *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*fill_res_srq_entry_raw)(struct sk_buff *, struct ib_srq *)</code>
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
