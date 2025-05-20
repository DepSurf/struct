# Struct: <code>mmc_request</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    void (*done)(struct mmc_request *);
    struct mmc_host *host;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    void (*done)(struct mmc_request *);
    struct mmc_host *host;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
    bool crypto_enabled;
    int crypto_key_slot;
    u32 data_unit_num;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
    const struct bio_crypt_ctx *crypto_ctx;
    int crypto_key_slot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
    const struct bio_crypt_ctx *crypto_ctx;
    int crypto_key_slot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
    const struct bio_crypt_ctx *crypto_ctx;
    int crypto_key_slot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
    const struct bio_crypt_ctx *crypto_ctx;
    int crypto_key_slot;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
    const struct bio_crypt_ctx *crypto_ctx;
    int crypto_key_slot;
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
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
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
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
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
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct mmc_request {
    struct mmc_command *sbc;
    struct mmc_command *cmd;
    struct mmc_data *data;
    struct mmc_command *stop;
    struct completion completion;
    struct completion cmd_completion;
    void (*done)(struct mmc_request *);
    void (*recovery_notifier)(struct mmc_request *);
    struct mmc_host *host;
    bool cap_cmd_during_tfr;
    int tag;
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
<details>
<summary>Changed between <code>4.8</code> and <code>4.10</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>struct completion cmd_completion</code>
</li>
<li>
<b>Field added. </b>
<code>bool cap_cmd_during_tfr</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.10</code> and <code>4.13</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.13</code> and <code>4.15</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>void (*recovery_notifier)(struct mmc_request *)</code>
</li>
<li>
<b>Field added. </b>
<code>int tag</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.11</code> and <code>5.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool crypto_enabled</code>
</li>
<li>
<b>Field added. </b>
<code>int crypto_key_slot</code>
</li>
<li>
<b>Field added. </b>
<code>u32 data_unit_num</code>
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
<code>const struct bio_crypt_ctx *crypto_ctx</code>
</li>
<li>
<b>Field removed. </b>
<code>bool crypto_enabled</code>
</li>
<li>
<b>Field removed. </b>
<code>u32 data_unit_num</code>
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
