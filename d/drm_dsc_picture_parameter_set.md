# Struct: <code>drm_dsc_picture_parameter_set</code>

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
In <code>4.10</code>: Absent ⚠️
</li>
<li>
In <code>4.13</code>: Absent ⚠️
</li>
<li>
In <code>4.15</code>: Absent ⚠️
</li>
<li>
In <code>4.18</code>: Absent ⚠️
</li>
<li>
In <code>5.0</code>: Absent ⚠️
</li>
<li>
In <code>5.3</code>: Absent ⚠️
</li>
<li>
In <code>5.4</code>: Absent ⚠️
</li>
<li>
<details>
<summary>In <code>5.8</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.11</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.13</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.15</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>5.19</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.2</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.5</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
<li>
<details>
<summary>In <code>6.8</code>: ✅</summary>

```c
struct drm_dsc_picture_parameter_set {
    u8 dsc_version;
    u8 pps_identifier;
    u8 pps_reserved;
    u8 pps_3;
    u8 pps_4;
    u8 bits_per_pixel_low;
    __be16 pic_height;
    __be16 pic_width;
    __be16 slice_height;
    __be16 slice_width;
    __be16 chunk_size;
    u8 initial_xmit_delay_high;
    u8 initial_xmit_delay_low;
    __be16 initial_dec_delay;
    u8 pps20_reserved;
    u8 initial_scale_value;
    __be16 scale_increment_interval;
    u8 scale_decrement_interval_high;
    u8 scale_decrement_interval_low;
    u8 pps26_reserved;
    u8 first_line_bpg_offset;
    __be16 nfl_bpg_offset;
    __be16 slice_bpg_offset;
    __be16 initial_offset;
    __be16 final_offset;
    u8 flatness_min_qp;
    u8 flatness_max_qp;
    __be16 rc_model_size;
    u8 rc_edge_factor;
    u8 rc_quant_incr_limit0;
    u8 rc_quant_incr_limit1;
    u8 rc_tgt_offset;
    u8 rc_buf_thresh[14];
    __be16 rc_range_parameters[15];
    u8 native_422_420;
    u8 second_line_bpg_offset;
    __be16 nsl_bpg_offset;
    __be16 second_line_offset_adj;
    u32 pps_long_94_reserved;
    u32 pps_long_98_reserved;
    u32 pps_long_102_reserved;
    u32 pps_long_106_reserved;
    u32 pps_long_110_reserved;
    u32 pps_long_114_reserved;
    u32 pps_long_118_reserved;
    u32 pps_long_122_reserved;
    __be16 pps_short_126_reserved;
};
```
</details>
</li>
</ul>
<b>Arch</b>
<ul>
<li>
In <code>arm64</code>: Absent ⚠️
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
In <code>aws</code>: Absent ⚠️
</li>
<li>
In <code>azure</code>: Absent ⚠️
</li>
<li>
In <code>gcp</code>: Absent ⚠️
</li>
<li>
In <code>lowlatency</code>: Absent ⚠️
</li>
</ul>

## Differences
<b>Regular</b>
<ul>
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
