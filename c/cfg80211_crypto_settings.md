# Struct: <code>cfg80211_crypto_settings</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    struct key_params *wep_keys;
    int wep_tx_key;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
    enum nl80211_sae_pwe_mechanism sae_pwe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
    enum nl80211_sae_pwe_mechanism sae_pwe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
    enum nl80211_sae_pwe_mechanism sae_pwe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
    enum nl80211_sae_pwe_mechanism sae_pwe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[10];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
    enum nl80211_sae_pwe_mechanism sae_pwe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[10];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
    enum nl80211_sae_pwe_mechanism sae_pwe;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[10];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    bool control_port_no_preauth;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
    enum nl80211_sae_pwe_mechanism sae_pwe;
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
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
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
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cfg80211_crypto_settings {
    u32 wpa_versions;
    u32 cipher_group;
    int n_ciphers_pairwise;
    u32 ciphers_pairwise[5];
    int n_akm_suites;
    u32 akm_suites[2];
    bool control_port;
    __be16 control_port_ethertype;
    bool control_port_no_encrypt;
    bool control_port_over_nl80211;
    struct key_params *wep_keys;
    int wep_tx_key;
    const u8 *psk;
    const u8 *sae_pwd;
    u8 sae_pwd_len;
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
<code>struct key_params *wep_keys</code>
</li>
<li>
<b>Field added. </b>
<code>int wep_tx_key</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const u8 *psk</code>
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
<code>bool control_port_over_nl80211</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.18</code> and <code>5.0</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>const u8 *sae_pwd</code>
</li>
<li>
<b>Field added. </b>
<code>u8 sae_pwd_len</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>5.4</code> and <code>5.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool control_port_no_preauth</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>enum nl80211_sae_pwe_mechanism sae_pwe</code>
</li>
</ul>
</details>
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
<b>Field type changed. </b>
<code>u32 akm_suites[2]</code> ➡️ <code>u32 akm_suites[10]</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>6.2</code> and <code>6.5</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>struct key_params *wep_keys</code>
</li>
<li>
<b>Field removed. </b>
<code>int wep_tx_key</code>
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
