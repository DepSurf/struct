# Struct: <code>disklabel</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
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
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
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
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct disklabel {
    __le32 d_magic;
    __le16 d_type;
    __le16 d_subtype;
    u8 d_typename[16];
    u8 d_packname[16];
    __le32 d_secsize;
    __le32 d_nsectors;
    __le32 d_ntracks;
    __le32 d_ncylinders;
    __le32 d_secpercyl;
    __le32 d_secprtunit;
    __le16 d_sparespertrack;
    __le16 d_sparespercyl;
    __le32 d_acylinders;
    __le16 d_rpm;
    __le16 d_interleave;
    __le16 d_trackskew;
    __le16 d_cylskew;
    __le32 d_headswitch;
    __le32 d_trkseek;
    __le32 d_flags;
    __le32 d_drivedata[5];
    __le32 d_spare[5];
    __le32 d_magic2;
    __le16 d_checksum;
    __le16 d_npartitions;
    __le32 d_bbsize;
    __le32 d_sbsize;
    struct d_partition d_partitions[18];
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
