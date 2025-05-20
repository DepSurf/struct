# Struct: <code>vas_winctx</code>

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
In <code>6.2</code>: Absent ⚠️
</li>
<li>
In <code>6.5</code>: Absent ⚠️
</li>
<li>
In <code>6.8</code>: Absent ⚠️
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
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct vas_winctx {
    void *rx_fifo;
    int rx_fifo_size;
    int wcreds_max;
    int rsvd_txbuf_count;
    bool user_win;
    bool nx_win;
    bool fault_win;
    bool rsvd_txbuf_enable;
    bool pin_win;
    bool rej_no_credit;
    bool tx_wcred_mode;
    bool rx_wcred_mode;
    bool tx_word_mode;
    bool rx_word_mode;
    bool data_stamp;
    bool xtra_write;
    bool notify_disable;
    bool intr_disable;
    bool fifo_disable;
    bool notify_early;
    bool notify_os_intr_reg;
    int lpid;
    int pidr;
    int lnotify_lpid;
    int lnotify_pid;
    int lnotify_tid;
    u32 pswid;
    int rx_win_id;
    int fault_win_id;
    int tc_mode;
    u64 irq_port;
    enum vas_dma_type dma_type;
    enum vas_notify_scope min_scope;
    enum vas_notify_scope max_scope;
    enum vas_notify_after_count notify_after_count;
};
```
</details>
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
<b>Arch</b>
<ul>
</ul>
