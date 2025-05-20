# Struct: <code>rpc_credops</code>

## Status
<b>Regular</b>
<ul>
<li>
In <code>4.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    struct rpc_cred * (*crbind)(struct rpc_task *, struct rpc_cred *, int);
    __be32 * (*crmarshal)(struct rpc_task *, __be32 *);
    int (*crrefresh)(struct rpc_task *);
    __be32 * (*crvalidate)(struct rpc_task *, __be32 *);
    int (*crwrap_req)(struct rpc_task *, kxdreproc_t, void *, __be32 *, void *);
    int (*crunwrap_resp)(struct rpc_task *, kxdrdproc_t, void *, __be32 *, void *);
    int (*crkey_timeout)(struct rpc_cred *);
    bool (*crkey_to_expire)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    struct rpc_cred * (*crbind)(struct rpc_task *, struct rpc_cred *, int);
    __be32 * (*crmarshal)(struct rpc_task *, __be32 *);
    int (*crrefresh)(struct rpc_task *);
    __be32 * (*crvalidate)(struct rpc_task *, __be32 *);
    int (*crwrap_req)(struct rpc_task *, kxdreproc_t, void *, __be32 *, void *);
    int (*crunwrap_resp)(struct rpc_task *, kxdrdproc_t, void *, __be32 *, void *);
    int (*crkey_timeout)(struct rpc_cred *);
    bool (*crkey_to_expire)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    struct rpc_cred * (*crbind)(struct rpc_task *, struct rpc_cred *, int);
    __be32 * (*crmarshal)(struct rpc_task *, __be32 *);
    int (*crrefresh)(struct rpc_task *);
    __be32 * (*crvalidate)(struct rpc_task *, __be32 *);
    int (*crwrap_req)(struct rpc_task *, kxdreproc_t, void *, __be32 *, void *);
    int (*crunwrap_resp)(struct rpc_task *, kxdrdproc_t, void *, __be32 *, void *);
    int (*crkey_timeout)(struct rpc_cred *);
    bool (*crkey_to_expire)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    struct rpc_cred * (*crbind)(struct rpc_task *, struct rpc_cred *, int);
    __be32 * (*crmarshal)(struct rpc_task *, __be32 *);
    int (*crrefresh)(struct rpc_task *);
    __be32 * (*crvalidate)(struct rpc_task *, __be32 *);
    int (*crwrap_req)(struct rpc_task *, kxdreproc_t, void *, __be32 *, void *);
    int (*crunwrap_resp)(struct rpc_task *, kxdrdproc_t, void *, __be32 *, void *);
    int (*crkey_timeout)(struct rpc_cred *);
    bool (*crkey_to_expire)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    struct rpc_cred * (*crbind)(struct rpc_task *, struct rpc_cred *, int);
    __be32 * (*crmarshal)(struct rpc_task *, __be32 *);
    int (*crrefresh)(struct rpc_task *);
    __be32 * (*crvalidate)(struct rpc_task *, __be32 *);
    int (*crwrap_req)(struct rpc_task *, kxdreproc_t, void *, __be32 *, void *);
    int (*crunwrap_resp)(struct rpc_task *, kxdrdproc_t, void *, __be32 *, void *);
    int (*crkey_timeout)(struct rpc_cred *);
    bool (*crkey_to_expire)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    __be32 * (*crmarshal)(struct rpc_task *, __be32 *);
    int (*crrefresh)(struct rpc_task *);
    __be32 * (*crvalidate)(struct rpc_task *, __be32 *);
    int (*crwrap_req)(struct rpc_task *, kxdreproc_t, void *, __be32 *, void *);
    int (*crunwrap_resp)(struct rpc_task *, kxdrdproc_t, void *, __be32 *, void *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
In <code>5.8</code>: Absent ⚠️
</li>
<li>
In <code>5.11</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
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
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
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
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct rpc_credops {
    const char *cr_name;
    int (*cr_init)(struct rpc_auth *, struct rpc_cred *);
    void (*crdestroy)(struct rpc_cred *);
    int (*crmatch)(struct auth_cred *, struct rpc_cred *, int);
    int (*crmarshal)(struct rpc_task *, struct xdr_stream *);
    int (*crrefresh)(struct rpc_task *);
    int (*crvalidate)(struct rpc_task *, struct xdr_stream *);
    int (*crwrap_req)(struct rpc_task *, struct xdr_stream *);
    int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *);
    int (*crkey_timeout)(struct rpc_cred *);
    char * (*crstringify_acceptor)(struct rpc_cred *);
    bool (*crneed_reencode)(struct rpc_task *);
};
```
</details>
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
<details>
<summary>Changed between <code>4.18</code> and <code>5.0</code> ⚠️</summary>
<ul>
<li>
<b>Field added. </b>
<code>bool (*crneed_reencode)(struct rpc_task *)</code>
</li>
<li>
<b>Field removed. </b>
<code>struct rpc_cred * (*crbind)(struct rpc_task *, struct rpc_cred *, int)</code>
</li>
<li>
<b>Field removed. </b>
<code>bool (*crkey_to_expire)(struct rpc_cred *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.0</code> and <code>5.3</code> ⚠️</summary>
<ul>
<li>
<b>Field type changed. </b>
<code>__be32 * (*crmarshal)(struct rpc_task *, __be32 *)</code> ➡️ <code>int (*crmarshal)(struct rpc_task *, struct xdr_stream *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>__be32 * (*crvalidate)(struct rpc_task *, __be32 *)</code> ➡️ <code>int (*crvalidate)(struct rpc_task *, struct xdr_stream *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*crwrap_req)(struct rpc_task *, kxdreproc_t, void *, __be32 *, void *)</code> ➡️ <code>int (*crwrap_req)(struct rpc_task *, struct xdr_stream *)</code>
</li>
<li>
<b>Field type changed. </b>
<code>int (*crunwrap_resp)(struct rpc_task *, kxdrdproc_t, void *, __be32 *, void *)</code> ➡️ <code>int (*crunwrap_resp)(struct rpc_task *, struct xdr_stream *)</code>
</li>
</ul>
</details>
</li>
<li>
No changes between <code>5.3</code> and <code>5.4</code> ✅
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
