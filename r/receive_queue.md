# Struct: <code>receive_queue</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct receive_queue {
    struct virtqueue *vq;
    struct napi_struct napi;
    struct page *pages;
    struct ewma_pkt_len mrg_avg_pkt_len;
    struct page_frag alloc_frag;
    struct scatterlist sg[19];
    char name[40];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct receive_queue {
    struct virtqueue *vq;
    struct napi_struct napi;
    struct page *pages;
    struct ewma_pkt_len mrg_avg_pkt_len;
    struct page_frag alloc_frag;
    struct scatterlist sg[19];
    char name[40];
};
```
</details>
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
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct receive_queue {
    struct virtqueue *vq;
    struct napi_struct napi;
    struct bpf_prog *xdp_prog;
    struct virtnet_rq_stats stats;
    struct page *pages;
    struct ewma_pkt_len mrg_avg_pkt_len;
    struct page_frag alloc_frag;
    struct scatterlist sg[19];
    unsigned int min_buf_len;
    char name[16];
    struct xdp_rxq_info xdp_rxq;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct receive_queue {
    struct virtqueue *vq;
    struct napi_struct napi;
    struct bpf_prog *xdp_prog;
    struct virtnet_rq_stats stats;
    u16 calls;
    bool dim_enabled;
    struct dim dim;
    u32 packets_in_napi;
    struct virtnet_interrupt_coalesce intr_coal;
    struct page *pages;
    struct ewma_pkt_len mrg_avg_pkt_len;
    struct page_frag alloc_frag;
    struct scatterlist sg[19];
    unsigned int min_buf_len;
    char name[16];
    struct xdp_rxq_info xdp_rxq;
    struct virtnet_rq_dma *last_dma;
    bool do_dma;
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
No changes between <code>4.4</code> and <code>4.8</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u16 calls</code>
</li>
<li>
<b>Field added. </b>
<code>bool dim_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>struct dim dim</code>
</li>
<li>
<b>Field added. </b>
<code>u32 packets_in_napi</code>
</li>
<li>
<b>Field added. </b>
<code>struct virtnet_interrupt_coalesce intr_coal</code>
</li>
<li>
<b>Field added. </b>
<code>struct virtnet_rq_dma *last_dma</code>
</li>
<li>
<b>Field added. </b>
<code>bool do_dma</code>
</li>
</ul>
</details>
</li>
</ul>
