# Struct: <code>rate_sample</code>

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
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rate_sample {
    struct skb_mstamp prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    u32 prior_delivered_ce;
    s32 delivered;
    s32 delivered_ce;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    u32 last_end_seq;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    u32 prior_delivered_ce;
    s32 delivered;
    s32 delivered_ce;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    u32 last_end_seq;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    u32 prior_delivered_ce;
    s32 delivered;
    s32 delivered_ce;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    u32 last_end_seq;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    u32 prior_delivered_ce;
    s32 delivered;
    s32 delivered_ce;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    u32 last_end_seq;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
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
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
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
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rate_sample {
    u64 prior_mstamp;
    u32 prior_delivered;
    s32 delivered;
    long int interval_us;
    u32 snd_interval_us;
    u32 rcv_interval_us;
    long int rtt_us;
    int losses;
    u32 acked_sacked;
    u32 prior_in_flight;
    bool is_app_limited;
    bool is_retrans;
    bool is_ack_delayed;
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
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>struct skb_mstamp prior_mstamp</code> ➡️ <code>u64 prior_mstamp</code>
</li>
</ul>
</details>
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
<code>bool is_ack_delayed</code>
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
<code>u32 snd_interval_us</code>
</li>
<li>
<b>Field added. </b>
<code>u32 rcv_interval_us</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>u32 prior_delivered_ce</code>
</li>
<li>
<b>Field added. </b>
<code>s32 delivered_ce</code>
</li>
<li>
<b>Field added. </b>
<code>u32 last_end_seq</code>
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
