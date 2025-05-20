# Struct: <code>macsec_ops</code>

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
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
In <code>5.13</code>: Absent ⚠️
</li>
<li>
In <code>5.15</code>: Absent ⚠️
</li>
<li>
In <code>5.19</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct macsec_ops {
    int (*mdo_dev_open)(struct macsec_context *);
    int (*mdo_dev_stop)(struct macsec_context *);
    int (*mdo_add_secy)(struct macsec_context *);
    int (*mdo_upd_secy)(struct macsec_context *);
    int (*mdo_del_secy)(struct macsec_context *);
    int (*mdo_add_rxsc)(struct macsec_context *);
    int (*mdo_upd_rxsc)(struct macsec_context *);
    int (*mdo_del_rxsc)(struct macsec_context *);
    int (*mdo_add_rxsa)(struct macsec_context *);
    int (*mdo_upd_rxsa)(struct macsec_context *);
    int (*mdo_del_rxsa)(struct macsec_context *);
    int (*mdo_add_txsa)(struct macsec_context *);
    int (*mdo_upd_txsa)(struct macsec_context *);
    int (*mdo_del_txsa)(struct macsec_context *);
    int (*mdo_get_dev_stats)(struct macsec_context *);
    int (*mdo_get_tx_sc_stats)(struct macsec_context *);
    int (*mdo_get_tx_sa_stats)(struct macsec_context *);
    int (*mdo_get_rx_sc_stats)(struct macsec_context *);
    int (*mdo_get_rx_sa_stats)(struct macsec_context *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct macsec_ops {
    int (*mdo_dev_open)(struct macsec_context *);
    int (*mdo_dev_stop)(struct macsec_context *);
    int (*mdo_add_secy)(struct macsec_context *);
    int (*mdo_upd_secy)(struct macsec_context *);
    int (*mdo_del_secy)(struct macsec_context *);
    int (*mdo_add_rxsc)(struct macsec_context *);
    int (*mdo_upd_rxsc)(struct macsec_context *);
    int (*mdo_del_rxsc)(struct macsec_context *);
    int (*mdo_add_rxsa)(struct macsec_context *);
    int (*mdo_upd_rxsa)(struct macsec_context *);
    int (*mdo_del_rxsa)(struct macsec_context *);
    int (*mdo_add_txsa)(struct macsec_context *);
    int (*mdo_upd_txsa)(struct macsec_context *);
    int (*mdo_del_txsa)(struct macsec_context *);
    int (*mdo_get_dev_stats)(struct macsec_context *);
    int (*mdo_get_tx_sc_stats)(struct macsec_context *);
    int (*mdo_get_tx_sa_stats)(struct macsec_context *);
    int (*mdo_get_rx_sc_stats)(struct macsec_context *);
    int (*mdo_get_rx_sa_stats)(struct macsec_context *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct macsec_ops {
    int (*mdo_dev_open)(struct macsec_context *);
    int (*mdo_dev_stop)(struct macsec_context *);
    int (*mdo_add_secy)(struct macsec_context *);
    int (*mdo_upd_secy)(struct macsec_context *);
    int (*mdo_del_secy)(struct macsec_context *);
    int (*mdo_add_rxsc)(struct macsec_context *);
    int (*mdo_upd_rxsc)(struct macsec_context *);
    int (*mdo_del_rxsc)(struct macsec_context *);
    int (*mdo_add_rxsa)(struct macsec_context *);
    int (*mdo_upd_rxsa)(struct macsec_context *);
    int (*mdo_del_rxsa)(struct macsec_context *);
    int (*mdo_add_txsa)(struct macsec_context *);
    int (*mdo_upd_txsa)(struct macsec_context *);
    int (*mdo_del_txsa)(struct macsec_context *);
    int (*mdo_get_dev_stats)(struct macsec_context *);
    int (*mdo_get_tx_sc_stats)(struct macsec_context *);
    int (*mdo_get_tx_sa_stats)(struct macsec_context *);
    int (*mdo_get_rx_sc_stats)(struct macsec_context *);
    int (*mdo_get_rx_sa_stats)(struct macsec_context *);
    int (*mdo_insert_tx_tag)(struct phy_device *, struct sk_buff *);
    unsigned int needed_headroom;
    unsigned int needed_tailroom;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
</li>
<li>
In <code>armhf</code>: Absent ⚠️
</li>
<li>
In <code>ppc64el</code>: Absent ⚠️
</li>
<li>
In <code>riscv64</code>: Absent ⚠️
</li>
</ul>
<b>Flavor</b>
<ul>
<li>
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
<li>
No changes between <code>6.2</code> and <code>6.5</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>int (*mdo_insert_tx_tag)(struct phy_device *, struct sk_buff *)</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int needed_headroom</code>
</li>
<li>
<b>Field added. </b>
<code>unsigned int needed_tailroom</code>
</li>
</ul>
</details>
</li>
</ul>
