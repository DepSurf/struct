# Struct: <code>macsec_secy</code>

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
struct macsec_secy {
    struct net_device *netdev;
    unsigned int n_rx_sc;
    sci_t sci;
    u16 key_len;
    u16 icv_len;
    enum macsec_validation_type validate_frames;
    bool xpn;
    bool operational;
    bool protect_frames;
    bool replay_protect;
    u32 replay_window;
    struct macsec_tx_sc tx_sc;
    struct macsec_rx_sc *rx_sc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct macsec_secy {
    struct net_device *netdev;
    unsigned int n_rx_sc;
    sci_t sci;
    u16 key_len;
    u16 icv_len;
    enum macsec_validation_type validate_frames;
    bool xpn;
    bool operational;
    bool protect_frames;
    bool replay_protect;
    u32 replay_window;
    struct macsec_tx_sc tx_sc;
    struct macsec_rx_sc *rx_sc;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct macsec_secy {
    struct net_device *netdev;
    unsigned int n_rx_sc;
    sci_t sci;
    u16 key_len;
    u16 icv_len;
    enum macsec_validation_type validate_frames;
    bool xpn;
    bool operational;
    bool protect_frames;
    bool replay_protect;
    u32 replay_window;
    struct macsec_tx_sc tx_sc;
    struct macsec_rx_sc *rx_sc;
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
No changes between <code>6.5</code> and <code>6.8</code> ✅
</li>
</ul>
