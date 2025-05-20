# Struct: <code>fc_host_statistics</code>

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
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct fc_host_statistics {
    u64 seconds_since_last_reset;
    u64 tx_frames;
    u64 tx_words;
    u64 rx_frames;
    u64 rx_words;
    u64 lip_count;
    u64 nos_count;
    u64 error_frames;
    u64 dumped_frames;
    u64 link_failure_count;
    u64 loss_of_sync_count;
    u64 loss_of_signal_count;
    u64 prim_seq_protocol_err_count;
    u64 invalid_tx_word_count;
    u64 invalid_crc_count;
    u64 fcp_input_requests;
    u64 fcp_output_requests;
    u64 fcp_control_requests;
    u64 fcp_input_megabytes;
    u64 fcp_output_megabytes;
    u64 fcp_packet_alloc_failures;
    u64 fcp_packet_aborts;
    u64 fcp_frame_alloc_failures;
    u64 fc_no_free_exch;
    u64 fc_no_free_exch_xid;
    u64 fc_xid_not_found;
    u64 fc_xid_busy;
    u64 fc_seq_not_found;
    u64 fc_non_bls_resp;
};
```
</details>
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Flavor</b>
<ul>
</ul>
