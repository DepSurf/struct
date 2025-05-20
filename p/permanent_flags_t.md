# Struct: <code>permanent_flags_t</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
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
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
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
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct permanent_flags_t {
    __be16 tag;
    u8 disable;
    u8 ownership;
    u8 deactivated;
    u8 readPubek;
    u8 disableOwnerClear;
    u8 allowMaintenance;
    u8 physicalPresenceLifetimeLock;
    u8 physicalPresenceHWEnable;
    u8 physicalPresenceCMDEnable;
    u8 CEKPUsed;
    u8 TPMpost;
    u8 TPMpostLock;
    u8 FIPS;
    u8 operator;
    u8 enableRevokeEK;
    u8 nvLocked;
    u8 readSRKPub;
    u8 tpmEstablished;
    u8 maintenanceDone;
    u8 disableFullDALogicInfo;
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
No changes between <code>generic</code> and <code>azure</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>gcp</code> ✅
</li>
<li>
No changes between <code>generic</code> and <code>lowlatency</code> ✅
</li>
</ul>
