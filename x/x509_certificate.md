# Struct: <code>x509_certificate</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    struct asymmetric_key_id *akid_id;
    struct asymmetric_key_id *akid_skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool trusted;
    bool unsupported_crypto;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_sig;
    bool blacklisted;
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
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
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
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct x509_certificate {
    struct x509_certificate *next;
    struct x509_certificate *signer;
    struct public_key *pub;
    struct public_key_signature *sig;
    char *issuer;
    char *subject;
    struct asymmetric_key_id *id;
    struct asymmetric_key_id *skid;
    time64_t valid_from;
    time64_t valid_to;
    const void *tbs;
    unsigned int tbs_size;
    unsigned int raw_sig_size;
    const void *raw_sig;
    const void *raw_serial;
    unsigned int raw_serial_size;
    unsigned int raw_issuer_size;
    const void *raw_issuer;
    const void *raw_subject;
    unsigned int raw_subject_size;
    unsigned int raw_skid_size;
    const void *raw_skid;
    unsigned int index;
    bool seen;
    bool verified;
    bool self_signed;
    bool unsupported_key;
    bool unsupported_sig;
    bool blacklisted;
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
<summary>Changed between <code>4.4</code> and <code>4.8</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool self_signed</code>
</li>
<li>
<b>Field added. </b>
<code>bool unsupported_key</code>
</li>
<li>
<b>Field added. </b>
<code>bool unsupported_sig</code>
</li>
<li>
<b>Field removed. </b>
<code>struct asymmetric_key_id *akid_id</code>
</li>
<li>
<b>Field removed. </b>
<code>struct asymmetric_key_id *akid_skid</code>
</li>
<li>
<b>Field removed. </b>
<code>bool trusted</code>
</li>
<li>
<b>Field removed. </b>
<code>bool unsupported_crypto</code>
</li>
<li>
<b>Field type changed. </b>
<code>struct public_key_signature sig</code> ➡️ <code>struct public_key_signature *sig</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>4.8</code> and <code>4.10</code> ✅
</li>
<li>
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool blacklisted</code>
</li>
</ul>
</details>
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
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>bool unsupported_key</code>
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
