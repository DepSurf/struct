# Struct: <code>ed</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
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
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
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
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
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
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct ed {
    __hc32 hwINFO;
    __hc32 hwTailP;
    __hc32 hwHeadP;
    __hc32 hwNextED;
    dma_addr_t dma;
    struct td *dummy;
    struct ed *ed_next;
    struct ed *ed_prev;
    struct list_head td_list;
    struct list_head in_use_list;
    u8 state;
    u8 type;
    u8 branch;
    u16 interval;
    u16 load;
    u16 last_iso;
    u16 tick;
    unsigned int takeback_wdh_cnt;
    struct td *pending_td;
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
No changes between <code>5.13</code> and <code>5.15</code> ✅
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
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
