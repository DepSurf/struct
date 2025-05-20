# Struct: <code>dcbnl_rtnl_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setapptrust)(struct net_device *, u8 *, int);
    int (*dcbnl_getapptrust)(struct net_device *, u8 *, int *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setapptrust)(struct net_device *, u8 *, int);
    int (*dcbnl_getapptrust)(struct net_device *, u8 *, int *);
    int (*dcbnl_setrewr)(struct net_device *, struct dcb_app *);
    int (*dcbnl_delrewr)(struct net_device *, struct dcb_app *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setapptrust)(struct net_device *, u8 *, int);
    int (*dcbnl_getapptrust)(struct net_device *, u8 *, int *);
    int (*dcbnl_setrewr)(struct net_device *, struct dcb_app *);
    int (*dcbnl_delrewr)(struct net_device *, struct dcb_app *);
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
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
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
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct dcbnl_rtnl_ops {
    int (*ieee_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_setets)(struct net_device *, struct ieee_ets *);
    int (*ieee_getmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_setmaxrate)(struct net_device *, struct ieee_maxrate *);
    int (*ieee_getqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_setqcn)(struct net_device *, struct ieee_qcn *);
    int (*ieee_getqcnstats)(struct net_device *, struct ieee_qcn_stats *);
    int (*ieee_getpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_setpfc)(struct net_device *, struct ieee_pfc *);
    int (*ieee_getapp)(struct net_device *, struct dcb_app *);
    int (*ieee_setapp)(struct net_device *, struct dcb_app *);
    int (*ieee_delapp)(struct net_device *, struct dcb_app *);
    int (*ieee_peer_getets)(struct net_device *, struct ieee_ets *);
    int (*ieee_peer_getpfc)(struct net_device *, struct ieee_pfc *);
    u8 (*getstate)(struct net_device *);
    u8 (*setstate)(struct net_device *, u8);
    void (*getpermhwaddr)(struct net_device *, u8 *);
    void (*setpgtccfgtx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgtx)(struct net_device *, int, u8);
    void (*setpgtccfgrx)(struct net_device *, int, u8, u8, u8, u8);
    void (*setpgbwgcfgrx)(struct net_device *, int, u8);
    void (*getpgtccfgtx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgtx)(struct net_device *, int, u8 *);
    void (*getpgtccfgrx)(struct net_device *, int, u8 *, u8 *, u8 *, u8 *);
    void (*getpgbwgcfgrx)(struct net_device *, int, u8 *);
    void (*setpfccfg)(struct net_device *, int, u8);
    void (*getpfccfg)(struct net_device *, int, u8 *);
    u8 (*setall)(struct net_device *);
    u8 (*getcap)(struct net_device *, int, u8 *);
    int (*getnumtcs)(struct net_device *, int, u8 *);
    int (*setnumtcs)(struct net_device *, int, u8);
    u8 (*getpfcstate)(struct net_device *);
    void (*setpfcstate)(struct net_device *, u8);
    void (*getbcncfg)(struct net_device *, int, u32 *);
    void (*setbcncfg)(struct net_device *, int, u32);
    void (*getbcnrp)(struct net_device *, int, u8 *);
    void (*setbcnrp)(struct net_device *, int, u8);
    int (*setapp)(struct net_device *, u8, u16, u8);
    int (*getapp)(struct net_device *, u8, u16);
    u8 (*getfeatcfg)(struct net_device *, int, u8 *);
    u8 (*setfeatcfg)(struct net_device *, int, u8);
    u8 (*getdcbx)(struct net_device *);
    u8 (*setdcbx)(struct net_device *, u8);
    int (*peer_getappinfo)(struct net_device *, struct dcb_peer_app_info *, u16 *);
    int (*peer_getapptable)(struct net_device *, struct dcb_app *);
    int (*cee_peer_getpg)(struct net_device *, struct cee_pg *);
    int (*cee_peer_getpfc)(struct net_device *, struct cee_pfc *);
    int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *);
    int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *);
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
<details>
<summary>Changed between <code>4.15</code> and <code>4.18</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*dcbnl_getbuffer)(struct net_device *, struct dcbnl_buffer *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dcbnl_setbuffer)(struct net_device *, struct dcbnl_buffer *)</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.19</code> and <code>6.2</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*dcbnl_setapptrust)(struct net_device *, u8 *, int)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dcbnl_getapptrust)(struct net_device *, u8 *, int *)</code>
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
<code>int (*dcbnl_setrewr)(struct net_device *, struct dcb_app *)</code>
</li>
<li>
<b>Field added. </b>
<code>int (*dcbnl_delrewr)(struct net_device *, struct dcb_app *)</code>
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
