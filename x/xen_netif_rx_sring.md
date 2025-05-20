# Struct: <code>xen_netif_rx_sring</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t __pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t __pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t __pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t __pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t __pad[48];
    union xen_netif_rx_sring_entry ring[0];
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
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
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
<details>
<summary>In <code>aws</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct xen_netif_rx_sring {
    RING_IDX req_prod;
    RING_IDX req_event;
    RING_IDX rsp_prod;
    RING_IDX rsp_event;
    uint8_t pad[48];
    union xen_netif_rx_sring_entry ring[1];
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
No changes between <code>4.15</code> and <code>4.18</code> ✅
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
<details>
<summary>Changed between <code>5.13</code> and <code>5.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>uint8_t __pad[48]</code>
</li>
<li>
<b>Field removed. </b>
<code>uint8_t pad[48]</code>
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
<details>
<summary>Changed between <code>6.5</code> and <code>6.8</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>union xen_netif_rx_sring_entry ring[1]</code> ➡️ <code>union xen_netif_rx_sring_entry ring[0]</code>
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
</ul>
<b>Flavor</b>
<ul>
<li>
No changes between <code>generic</code> and <code>aws</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
