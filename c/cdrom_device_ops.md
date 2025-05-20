# Struct: <code>cdrom_device_ops</code>

## Status
<b>Regular</b>
<ul>
<li>
<details>
<summary>In <code>4.4</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int n_minors;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.8</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int n_minors;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.10</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int n_minors;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.13</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.15</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>4.18</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.0</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.3</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.4</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
    int (*read_cdda_bpc)(struct cdrom_device_info *, void *, u32, u32, u8 *);
    const int capability;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
    int (*read_cdda_bpc)(struct cdrom_device_info *, void *, u32, u32, u8 *);
    const int capability;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
    int (*read_cdda_bpc)(struct cdrom_device_info *, void *, u32, u32, u8 *);
    const int capability;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
    int (*read_cdda_bpc)(struct cdrom_device_info *, void *, u32, u32, u8 *);
    const int capability;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
    int (*read_cdda_bpc)(struct cdrom_device_info *, void *, u32, u32, u8 *);
    const int capability;
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
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>armhf</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>ppc64el</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>riscv64</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
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
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>azure</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>gcp</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
};
```
</details>
</li>
<li>
<details>
<summary>In <code>lowlatency</code>: ✅</summary>

```c
struct cdrom_device_ops {
    int (*open)(struct cdrom_device_info *, int);
    void (*release)(struct cdrom_device_info *);
    int (*drive_status)(struct cdrom_device_info *, int);
    unsigned int (*check_events)(struct cdrom_device_info *, unsigned int, int);
    int (*media_changed)(struct cdrom_device_info *, int);
    int (*tray_move)(struct cdrom_device_info *, int);
    int (*lock_door)(struct cdrom_device_info *, int);
    int (*select_speed)(struct cdrom_device_info *, int);
    int (*select_disc)(struct cdrom_device_info *, int);
    int (*get_last_session)(struct cdrom_device_info *, struct cdrom_multisession *);
    int (*get_mcn)(struct cdrom_device_info *, struct cdrom_mcn *);
    int (*reset)(struct cdrom_device_info *);
    int (*audio_ioctl)(struct cdrom_device_info *, unsigned int, void *);
    const int capability;
    int (*generic_packet)(struct cdrom_device_info *, struct packet_command *);
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
<details>
<summary>Changed between <code>4.10</code> and <code>4.13</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int n_minors</code>
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
<details>
<summary>Changed between <code>5.8</code> and <code>5.11</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*media_changed)(struct cdrom_device_info *, int)</code>
</li>
</ul>
</details>
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
<code>int (*read_cdda_bpc)(struct cdrom_device_info *, void *, u32, u32, u8 *)</code>
</li>
</ul>
</details>
</li>
<li>
<details>
<summary>Changed between <code>5.15</code> and <code>5.19</code> ⚠️</summary>
<ul>
<li>
<b>Field removed. </b>
<code>int (*select_disc)(struct cdrom_device_info *, int)</code>
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
