# Inventář UltraGridu

Statický index výchozího commitu 59e89f6 a wiki 7855c72. Řádky ve zdrojových odkazech odpovídají dokumentační větvi.
Záznam v registru označuje implementaci v kódu. Podpora na konkrétním stroji závisí na sestavení, SDK, dynamických knihovnách a zařízení.
Výpis zahrnuje přímo čitelné registrace a volby. Aliasy, makra generující registrace a parametry jednotlivých modulů ověřit přes zdroj a nápovědu.

Výchozí strom má 1031 sledovaných položek. Níže je 177 přímo rozpoznaných registrací, 52 rozšířených parametrů, 46 dlouhých CLI voleb a 102 detekovaných voleb konfigurace.

## Moduly podle třídy

### AUDIO_CAPTURE

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `AESEBU` | `REGISTER_MODULE` | [src/audio/capture/sdi.c:263](../../src/audio/capture/sdi.c#L263) |
| `aes67` | `REGISTER_MODULE` | [src/audio/capture/aes67.cpp:576](../../src/audio/capture/aes67.cpp#L576) |
| `alsa` | `REGISTER_MODULE` | [src/audio/capture/alsa.c:422](../../src/audio/capture/alsa.c#L422) |
| `analog` | `REGISTER_MODULE` | [src/audio/capture/sdi.c:264](../../src/audio/capture/sdi.c#L264) |
| `coreaudio` | `REGISTER_MODULE` | [src/audio/capture/coreaudio.m:459](../../src/audio/capture/coreaudio.m#L459) |
| `embedded` | `REGISTER_MODULE` | [src/audio/capture/sdi.c:262](../../src/audio/capture/sdi.c#L262) |
| `fluidsynth` | `REGISTER_MODULE` | [src/audio/capture/fluidsynth.c:363](../../src/audio/capture/fluidsynth.c#L363) |
| `jack` | `REGISTER_MODULE` | [src/audio/capture/jack.c:327](../../src/audio/capture/jack.c#L327) |
| `none` | `REGISTER_MODULE` | [src/audio/capture/none.c:105](../../src/audio/capture/none.c#L105) |
| `passive` | `REGISTER_MODULE` | [src/audio/capture/passive.c:129](../../src/audio/capture/passive.c#L129) |
| `pipewire` | `REGISTER_MODULE` | [src/audio/capture/pipewire.cpp:345](../../src/audio/capture/pipewire.cpp#L345) |
| `portaudio` | `REGISTER_MODULE` | [src/audio/capture/portaudio.c:353](../../src/audio/capture/portaudio.c#L353) |
| `sdl_mixer` | `REGISTER_MODULE_WITH_FLAG` | [src/audio/capture/fluidsynth.c:365](../../src/audio/capture/fluidsynth.c#L365) |
| `testcard` | `REGISTER_MODULE` | [src/audio/capture/testcard.c:511](../../src/audio/capture/testcard.c#L511) |
| `wasapi` | `REGISTER_MODULE` | [src/audio/capture/wasapi.cpp:506](../../src/audio/capture/wasapi.cpp#L506) |
| `wav` | `REGISTER_MODULE` | [src/audio/capture/wav.c:178](../../src/audio/capture/wav.c#L178) |

### AUDIO_COMPRESS

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `dummy_pcm` | `REGISTER_MODULE` | [src/audio/codec/dummy_pcm.c:110](../../src/audio/codec/dummy_pcm.c#L110) |
| `libavcodec` | `REGISTER_MODULE` | [src/audio/codec/libavcodec.c:882](../../src/audio/codec/libavcodec.c#L882) |

### AUDIO_FILTER

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `channel_remap` | `REGISTER_MODULE` | [src/audio/filter/channel_remap.cpp:195](../../src/audio/filter/channel_remap.cpp#L195) |
| `compressor` | `REGISTER_MODULE` | [src/audio/filter/compressor.cpp:263](../../src/audio/filter/compressor.cpp#L263) |
| `controlport_stats` | `REGISTER_MODULE` | [src/audio/filter/controlport_stats.cpp:148](../../src/audio/filter/controlport_stats.cpp#L148) |
| `delay` | `REGISTER_MODULE` | [src/audio/filter/delay.cpp:213](../../src/audio/filter/delay.cpp#L213) |
| `playback` | `REGISTER_MODULE` | [src/audio/filter/playback.cpp:178](../../src/audio/filter/playback.cpp#L178) |
| `silence` | `REGISTER_MODULE` | [src/audio/filter/silence.c:172](../../src/audio/filter/silence.c#L172) |

### AUDIO_PLAYBACK

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `AESEBU` | `REGISTER_MODULE` | [src/audio/playback/sdi.c:203](../../src/audio/playback/sdi.c#L203) |
| `aes67` | `REGISTER_MODULE` | [src/audio/playback/aes67.cpp:570](../../src/audio/playback/aes67.cpp#L570) |
| `alsa` | `REGISTER_MODULE` | [src/audio/playback/alsa.c:1110](../../src/audio/playback/alsa.c#L1110) |
| `analog` | `REGISTER_MODULE` | [src/audio/playback/sdi.c:204](../../src/audio/playback/sdi.c#L204) |
| `coreaudio` | `REGISTER_MODULE` | [src/audio/playback/coreaudio.c:577](../../src/audio/playback/coreaudio.c#L577) |
| `decklink` | `REGISTER_MODULE` | [src/audio/playback/decklink.cpp:465](../../src/audio/playback/decklink.cpp#L465) |
| `dummy` | `REGISTER_MODULE` | [src/audio/playback/dummy.c:152](../../src/audio/playback/dummy.c#L152) |
| `dump` | `REGISTER_MODULE` | [src/audio/playback/dump.cpp:155](../../src/audio/playback/dump.cpp#L155) |
| `embedded` | `REGISTER_MODULE` | [src/audio/playback/sdi.c:202](../../src/audio/playback/sdi.c#L202) |
| `jack` | `REGISTER_MODULE` | [src/audio/playback/jack.c:407](../../src/audio/playback/jack.c#L407) |
| `mixer` | `REGISTER_MODULE` | [src/audio/playback/mixer.cpp:556](../../src/audio/playback/mixer.cpp#L556) |
| `none` | `REGISTER_MODULE` | [src/audio/playback/none.c:118](../../src/audio/playback/none.c#L118) |
| `pipewire` | `REGISTER_MODULE` | [src/audio/playback/pipewire.cpp:392](../../src/audio/playback/pipewire.cpp#L392) |
| `portaudio` | `REGISTER_MODULE` | [src/audio/playback/portaudio.c:501](../../src/audio/playback/portaudio.c#L501) |
| `wasapi` | `REGISTER_MODULE` | [src/audio/playback/wasapi.cpp:447](../../src/audio/playback/wasapi.cpp#L447) |

### CAPTURE_FILTER

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `add_frame` | `REGISTER_MODULE` | [src/capture_filter/add_frame.c:202](../../src/capture_filter/add_frame.c#L202) |
| `blank` | `REGISTER_MODULE` | [src/capture_filter/blank.c:309](../../src/capture_filter/blank.c#L309) |
| `change_pixfmt` | `REGISTER_MODULE` | [src/capture_filter/change_pixfmt.c:183](../../src/capture_filter/change_pixfmt.c#L183) |
| `color` | `REGISTER_MODULE` | [src/capture_filter/color.c:129](../../src/capture_filter/color.c#L129) |
| `crop` | `REGISTER_MODULE` | [src/vo_postprocess/crop.c:253](../../src/vo_postprocess/crop.c#L253) |
| `deinterlace` | `REGISTER_MODULE` | [src/vo_postprocess/deinterlace.c:245](../../src/vo_postprocess/deinterlace.c#L245) |
| `every` | `REGISTER_MODULE` | [src/capture_filter/every.c:186](../../src/capture_filter/every.c#L186) |
| `flip` | `REGISTER_MODULE` | [src/capture_filter/flip.c:118](../../src/capture_filter/flip.c#L118) |
| `gamma` | `REGISTER_MODULE` | [src/capture_filter/gamma.cpp:246](../../src/capture_filter/gamma.cpp#L246) |
| `grayscale` | `REGISTER_MODULE` | [src/capture_filter/grayscale.c:136](../../src/capture_filter/grayscale.c#L136) |
| `logo` | `REGISTER_MODULE` | [src/capture_filter/logo.c:243](../../src/capture_filter/logo.c#L243) |
| `matrix` | `REGISTER_MODULE` | [src/capture_filter/matrix.c:327](../../src/capture_filter/matrix.c#L327) |
| `matrix2` | `REGISTER_MODULE` | [src/capture_filter/matrix2.c:293](../../src/capture_filter/matrix2.c#L293) |
| `mirror` | `REGISTER_MODULE` | [src/capture_filter/mirror.c:141](../../src/capture_filter/mirror.c#L141) |
| `name` | `REGISTER_MODULE` | [src/capture_filter/vo_pp_wrapper.h:95](../../src/capture_filter/vo_pp_wrapper.h#L95) |
| `noise` | `REGISTER_MODULE` | [src/capture_filter/noise.c:172](../../src/capture_filter/noise.c#L172) |
| `override_prop` | `REGISTER_MODULE` | [src/capture_filter/override_prop.c:180](../../src/capture_filter/override_prop.c#L180) |
| `r1x_to_y416_fake` | `REGISTER_MODULE` | [src/capture_filter/r12l_to_y416_fake.c:263](../../src/capture_filter/r12l_to_y416_fake.c#L263) |
| `ratelimit` | `REGISTER_MODULE` | [src/capture_filter/ratelimit.c:127](../../src/capture_filter/ratelimit.c#L127) |
| `resize` | `REGISTER_MODULE` | [src/capture_filter/resize.c:288](../../src/capture_filter/resize.c#L288) |
| `split` | `REGISTER_MODULE` | [src/capture_filter/split.c:128](../../src/capture_filter/split.c#L128) |
| `temporal_3d` | `REGISTER_MODULE` | [src/capture_filter/temporal_3d.c:141](../../src/capture_filter/temporal_3d.c#L141) |
| `text` | `REGISTER_MODULE` | [src/vo_postprocess/text.c:537](../../src/vo_postprocess/text.c#L537) |

### RXTX

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `ihdtv` | `REGISTER_MODULE` | [src/rxtx/ihdtv.cpp:228](../../src/rxtx/ihdtv.cpp#L228) |
| `jack` | `REGISTER_MODULE` | [src/rxtx/jack_audio.c:125](../../src/rxtx/jack_audio.c#L125) |
| `loopback` | `REGISTER_MODULE` | [src/rxtx/loopback.c:383](../../src/rxtx/loopback.c#L383) |
| `mpegts` | `REGISTER_MODULE` | [src/rxtx/mpegts.c:588](../../src/rxtx/mpegts.c#L588) |
| `omt` | `REGISTER_MODULE` | [src/rxtx/omt.cpp:218](../../src/rxtx/omt.cpp#L218) |
| `rtsp` | `REGISTER_MODULE` | [src/rxtx/rtsp.c:368](../../src/rxtx/rtsp.c#L368) |
| `sage` | `REGISTER_MODULE` | [src/rxtx/sage.cpp:142](../../src/rxtx/sage.cpp#L142) |
| `sdp` | `REGISTER_MODULE` | [src/rxtx/h264_sdp.c:356](../../src/rxtx/h264_sdp.c#L356) |
| `ultragrid_rtp` | `REGISTER_MODULE` | [src/rxtx/ultragrid_rtp.c:681](../../src/rxtx/ultragrid_rtp.c#L681) |

### UNDEFINED

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `ldgm_gpu` | `REGISTER_MODULE` | [src/rtp/ldgm_gpu.cpp:9](../../src/rtp/ldgm_gpu.cpp#L9) |
| `openssl_decrypt` | `REGISTER_MODULE` | [src/crypto/openssl_decrypt.c:187](../../src/crypto/openssl_decrypt.c#L187) |
| `openssl_encrypt` | `REGISTER_MODULE` | [src/crypto/openssl_encrypt.c:277](../../src/crypto/openssl_encrypt.c#L277) |
| `udp_holepunch` | `REGISTER_MODULE` | [src/utils/udp_holepunch.cpp:378](../../src/utils/udp_holepunch.cpp#L378) |

### VIDEO_CAPTURE

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `aggregate` | `REGISTER_MODULE` | [src/video_capture/aggregate.c:241](../../src/video_capture/aggregate.c#L241) |
| `aja` | `REGISTER_MODULE` | [src/aja_win32_stub.c:45](../../src/aja_win32_stub.c#L45) |
| `aja` | `REGISTER_MODULE` | [src/video_capture/aja.cpp:1184](../../src/video_capture/aja.cpp#L1184) |
| `avfoundation` | `REGISTER_MODULE` | [src/video_capture/avfoundation.mm:836](../../src/video_capture/avfoundation.mm#L836) |
| `bitflow` | `REGISTER_MODULE` | [src/video_capture/bitflow.cpp:373](../../src/video_capture/bitflow.cpp#L373) |
| `bluefish444` | `REGISTER_MODULE` | [src/video_capture/bluefish444.cpp:1097](../../src/video_capture/bluefish444.cpp#L1097) |
| `decklink` | `REGISTER_MODULE` | [src/video_capture/decklink.cpp:2017](../../src/video_capture/decklink.cpp#L2017) |
| `deltacast` | `REGISTER_MODULE` | [src/video_capture/deltacast.cpp:670](../../src/video_capture/deltacast.cpp#L670) |
| `dshow` | `REGISTER_MODULE` | [src/video_capture/DirectShowGrabber.cpp:1441](../../src/video_capture/DirectShowGrabber.cpp#L1441) |
| `dvs` | `REGISTER_MODULE` | [src/video_capture.h:85](../../src/video_capture.h#L85) |
| `dvs` | `REGISTER_MODULE` | [src/video_capture/dvs.c:696](../../src/video_capture/dvs.c#L696) |
| `file` | `REGISTER_MODULE` | [src/video_capture/file.c:1084](../../src/video_capture/file.c#L1084) |
| `gpustitch` | `REGISTER_MODULE` | [src/video_capture/gpustitch.cpp:765](../../src/video_capture/gpustitch.cpp#L765) |
| `import` | `REGISTER_MODULE` | [src/video_capture/import.c:1178](../../src/video_capture/import.c#L1178) |
| `ndi` | `REGISTER_MODULE` | [src/video_capture/ndi.cpp:678](../../src/video_capture/ndi.cpp#L678) |
| `omt` | `REGISTER_MODULE` | [src/video_capture/omt.cpp:280](../../src/video_capture/omt.cpp#L280) |
| `pipewire` | `REGISTER_MODULE` | [src/video_capture/pipewire.cpp:648](../../src/video_capture/pipewire.cpp#L648) |
| `rtsp` | `REGISTER_MODULE` | [src/video_capture/rtsp.c:1330](../../src/video_capture/rtsp.c#L1330) |
| `screen` | `REGISTER_MODULE` | [src/video_capture/screen_avf.c:153](../../src/video_capture/screen_avf.c#L153) |
| `screen` | `REGISTER_MODULE` | [src/video_capture/screen_linux.c:128](../../src/video_capture/screen_linux.c#L128) |
| `screen` | `REGISTER_MODULE` | [src/video_capture/screen_osx.c:311](../../src/video_capture/screen_osx.c#L311) |
| `screen` | `REGISTER_MODULE` | [src/video_capture/screen_win.c:555](../../src/video_capture/screen_win.c#L555) |
| `screen_pw` | `REGISTER_MODULE` | [src/video_capture/pipewire.cpp:636](../../src/video_capture/pipewire.cpp#L636) |
| `screen_x11` | `REGISTER_MODULE` | [src/video_capture/screen_x11.c:489](../../src/video_capture/screen_x11.c#L489) |
| `spout` | `REGISTER_MODULE` | [src/video_capture/spout.cpp:342](../../src/video_capture/spout.cpp#L342) |
| `switcher` | `REGISTER_MODULE` | [src/video_capture/switcher.c:353](../../src/video_capture/switcher.c#L353) |
| `swmix` | `REGISTER_MODULE` | [src/video_capture/swmix.c:1356](../../src/video_capture/swmix.c#L1356) |
| `syphon` | `REGISTER_MODULE` | [src/video_capture/syphon.m:578](../../src/video_capture/syphon.m#L578) |
| `testcard` | `REGISTER_MODULE` | [src/video_capture/testcard.c:872](../../src/video_capture/testcard.c#L872) |
| `testcard2` | `REGISTER_MODULE` | [src/video_capture/testcard2.c:767](../../src/video_capture/testcard2.c#L767) |
| `ug_input` | `REGISTER_MODULE` | [src/video_capture/ug_input.c:297](../../src/video_capture/ug_input.c#L297) |
| `v4l2` | `REGISTER_MODULE` | [src/video_capture/v4l2.c:890](../../src/video_capture/v4l2.c#L890) |
| `ximea` | `REGISTER_MODULE` | [src/video_capture/ximea.c:350](../../src/video_capture/ximea.c#L350) |

### VIDEO_COMPRESS

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `cineform` | `REGISTER_MODULE` | [src/video_compress/cineform.cpp:544](../../src/video_compress/cineform.cpp#L544) |
| `cmpto_j2k` | `REGISTER_MODULE` | [src/video_compress/cmpto_j2k.cpp:1008](../../src/video_compress/cmpto_j2k.cpp#L1008) |
| `cuda_dxt` | `REGISTER_MODULE` | [src/video_compress/cuda_dxt.cpp:290](../../src/video_compress/cuda_dxt.cpp#L290) |
| `gpujpeg` | `REGISTER_MODULE` | [src/video_compress/gpujpeg.cpp:791](../../src/video_compress/gpujpeg.cpp#L791) |
| `jpegxs` | `REGISTER_MODULE` | [src/video_compress/jpegxs.cpp:620](../../src/video_compress/jpegxs.cpp#L620) |
| `libavcodec` | `REGISTER_MODULE` | [src/video_compress/libavcodec.cpp:2526](../../src/video_compress/libavcodec.cpp#L2526) |
| `none` | `REGISTER_MODULE` | [src/video_compress/none.cpp:97](../../src/video_compress/none.cpp#L97) |
| `openapv` | `REGISTER_MODULE` | [src/video_compress/openapv.cpp:426](../../src/video_compress/openapv.cpp#L426) |
| `pyrowave` | `REGISTER_MODULE` | [src/video_compress/pyrowave.cpp:250](../../src/video_compress/pyrowave.cpp#L250) |
| `rtdxt` | `REGISTER_MODULE` | [src/video_compress/dxt_glsl.cpp:332](../../src/video_compress/dxt_glsl.cpp#L332) |
| `uyvy` | `REGISTER_MODULE` | [src/video_compress/uyvy.cpp:304](../../src/video_compress/uyvy.cpp#L304) |

### VIDEO_DECOMPRESS

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `cineform` | `REGISTER_MODULE` | [src/video_decompress/cineform.cpp:435](../../src/video_decompress/cineform.cpp#L435) |
| `dxt_glsl` | `REGISTER_MODULE` | [src/video_decompress/dxt_glsl.c:248](../../src/video_decompress/dxt_glsl.c#L248) |
| `gpujpeg` | `REGISTER_MODULE` | [src/video_decompress/gpujpeg.c:378](../../src/video_decompress/gpujpeg.c#L378) |
| `gpujpeg_to_dxt` | `REGISTER_MODULE` | [src/video_decompress/gpujpeg_to_dxt.cpp:380](../../src/video_decompress/gpujpeg_to_dxt.cpp#L380) |
| `i420` | `REGISTER_MODULE` | [src/video_decompress/i420.c:129](../../src/video_decompress/i420.c#L129) |
| `j2k` | `REGISTER_MODULE` | [src/video_decompress/cmpto_j2k.cpp:801](../../src/video_decompress/cmpto_j2k.cpp#L801) |
| `jpegxs` | `REGISTER_MODULE` | [src/video_decompress/jpegxs.cpp:388](../../src/video_decompress/jpegxs.cpp#L388) |
| `libavcodec` | `REGISTER_MODULE` | [src/video_decompress/libavcodec.c:1226](../../src/video_decompress/libavcodec.c#L1226) |
| `openapv` | `REGISTER_MODULE` | [src/video_decompress/openapv.cpp:353](../../src/video_decompress/openapv.cpp#L353) |
| `pyrowave` | `REGISTER_MODULE` | [src/video_decompress/pyrowave.cpp:230](../../src/video_decompress/pyrowave.cpp#L230) |

### VIDEO_DISPLAY

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `NAME_SPOUT_SYPHON_RAW` | `REGISTER_MODULE` | [src/video_display/gl.c:2611](../../src/video_display/gl.c#L2611) |
| `aja` | `REGISTER_MODULE` | [src/aja_win32_stub.c:49](../../src/aja_win32_stub.c#L49) |
| `aja` | `REGISTER_MODULE` | [src/video_display/aja.cpp:1148](../../src/video_display/aja.cpp#L1148) |
| `bluefish444` | `REGISTER_MODULE` | [src/video_display/bluefish444.cpp:1049](../../src/video_display/bluefish444.cpp#L1049) |
| `caca` | `REGISTER_MODULE_WITH_FUNC` | [src/video_display/caca.c:348](../../src/video_display/caca.c#L348) |
| `decklink` | `REGISTER_MODULE` | [src/video_display/decklink.cpp:2294](../../src/video_display/decklink.cpp#L2294) |
| `deltacast` | `REGISTER_MODULE` | [src/video_display/deltacast.cpp:604](../../src/video_display/deltacast.cpp#L604) |
| `drm` | `REGISTER_MODULE` | [src/video_display/drm.cpp:1119](../../src/video_display/drm.cpp#L1119) |
| `dummy` | `REGISTER_MODULE` | [src/video_display/dummy.c:378](../../src/video_display/dummy.c#L378) |
| `dump` | `REGISTER_MODULE` | [src/video_display/dump.c:215](../../src/video_display/dump.c#L215) |
| `dvs` | `REGISTER_MODULE` | [src/video_display/dvs.c:999](../../src/video_display/dvs.c#L999) |
| `file` | `REGISTER_MODULE_WITH_FUNC` | [src/video_display/file.c:927](../../src/video_display/file.c#L927) |
| `gl` | `REGISTER_MODULE` | [src/video_display/gl.c:2576](../../src/video_display/gl.c#L2576) |
| `multiplier` | `REGISTER_MODULE` | [src/video_display/multiplier.cpp:301](../../src/video_display/multiplier.cpp#L301) |
| `ndi` | `REGISTER_MODULE` | [src/video_display/ndi.c:480](../../src/video_display/ndi.c#L480) |
| `omt` | `REGISTER_MODULE` | [src/video_display/omt.cpp:374](../../src/video_display/omt.cpp#L374) |
| `openxr_gl` | `REGISTER_MODULE` | [src/video_display/openxr_gl.cpp:1161](../../src/video_display/openxr_gl.cpp#L1161) |
| `pano_gl` | `REGISTER_MODULE` | [src/video_display/pano_gl.cpp:402](../../src/video_display/pano_gl.cpp#L402) |
| `pipewire` | `REGISTER_MODULE` | [src/video_display/pipewire.cpp:496](../../src/video_display/pipewire.cpp#L496) |
| `sage` | `REGISTER_MODULE` | [src/video_display/sage.cpp:563](../../src/video_display/sage.cpp#L563) |
| `sdl` | `REGISTER_MODULE` | [src/video_display/sdl.cpp:779](../../src/video_display/sdl.cpp#L779) |
| `sdl` | `REGISTER_MODULE` | [src/video_display/sdl2.c:1023](../../src/video_display/sdl2.c#L1023) |
| `sdl` | `REGISTER_MODULE` | [src/video_display/sdl3.c:1478](../../src/video_display/sdl3.c#L1478) |
| `sdl2` | `REGISTER_MODULE_WITH_FLAG` | [src/video_display/sdl2.c:1024](../../src/video_display/sdl2.c#L1024) |
| `sdl3` | `REGISTER_MODULE_WITH_FLAG` | [src/video_display/sdl3.c:1480](../../src/video_display/sdl3.c#L1480) |
| `v4l2` | `REGISTER_MODULE` | [src/video_display/v4l2.c:340](../../src/video_display/v4l2.c#L340) |
| `vulkan` | `REGISTER_MODULE` | [src/video_display/vulkan/vulkan_sdl3.cpp:1047](../../src/video_display/vulkan/vulkan_sdl3.cpp#L1047) |
| `vulkan` | `REGISTER_MODULE_WITH_FLAG` | [src/video_display/vulkan/vulkan_sdl2.cpp:1024](../../src/video_display/vulkan/vulkan_sdl2.cpp#L1024) |
| `vulkan_sdl2` | `REGISTER_MODULE` | [src/video_display/vulkan/vulkan_sdl2.cpp:1023](../../src/video_display/vulkan/vulkan_sdl2.cpp#L1023) |
| `vulkan_sdl3` | `REGISTER_MODULE_WITH_FLAG` | [src/video_display/vulkan/vulkan_sdl3.cpp:1048](../../src/video_display/vulkan/vulkan_sdl3.cpp#L1048) |

### VIDEO_POSTPROCESS

| Název | Registrace | Zdroj |
| --- | --- | --- |
| `add_frame` | `REGISTER_MODULE` | [src/vo_postprocess/add_frame.c:206](../../src/vo_postprocess/add_frame.c#L206) |
| `border` | `REGISTER_MODULE` | [src/vo_postprocess/border.c:246](../../src/vo_postprocess/border.c#L246) |
| `crop` | `REGISTER_MODULE` | [src/vo_postprocess/crop.c:252](../../src/vo_postprocess/crop.c#L252) |
| `deinterlace` | `REGISTER_MODULE` | [src/vo_postprocess/deinterlace.c:244](../../src/vo_postprocess/deinterlace.c#L244) |
| `deinterlace_blend` | `REGISTER_MODULE` | [src/vo_postprocess/deinterlace.c:243](../../src/vo_postprocess/deinterlace.c#L243) |
| `deinterlace_bob` | `REGISTER_MODULE` | [src/vo_postprocess/temporal-deint.c:573](../../src/vo_postprocess/temporal-deint.c#L573) |
| `deinterlace_linear` | `REGISTER_MODULE` | [src/vo_postprocess/temporal-deint.c:578](../../src/vo_postprocess/temporal-deint.c#L578) |
| `delay` | `REGISTER_MODULE` | [src/vo_postprocess/delay.c:216](../../src/vo_postprocess/delay.c#L216) |
| `double_framerate` | `REGISTER_MODULE` | [src/vo_postprocess/temporal-deint.c:568](../../src/vo_postprocess/temporal-deint.c#L568) |
| `dummy` | `REGISTER_MODULE` | [src/vo_postprocess/dummy.c:137](../../src/vo_postprocess/dummy.c#L137) |
| `interlace` | `REGISTER_MODULE` | [src/vo_postprocess/interlace.c:223](../../src/vo_postprocess/interlace.c#L223) |
| `interlaced_3d` | `REGISTER_MODULE` | [src/vo_postprocess/3d-interlaced.c:213](../../src/vo_postprocess/3d-interlaced.c#L213) |
| `name` | `REGISTER_MODULE` | [src/vo_postprocess/capture_filter_wrapper.h:155](../../src/vo_postprocess/capture_filter_wrapper.h#L155) |
| `scale` | `REGISTER_MODULE` | [src/vo_postprocess/scale.c:356](../../src/vo_postprocess/scale.c#L356) |
| `split` | `REGISTER_MODULE` | [src/vo_postprocess/split.c:196](../../src/vo_postprocess/split.c#L196) |
| `temporal_3d` | `REGISTER_MODULE` | [src/vo_postprocess/temporal_3d.c:230](../../src/vo_postprocess/temporal_3d.c#L230) |
| `text` | `REGISTER_MODULE` | [src/vo_postprocess/text.c:536](../../src/vo_postprocess/text.c#L536) |
| `y416_to_r1x_fake` | `REGISTER_MODULE` | [src/vo_postprocess/y416_to_r12l_fake.c:341](../../src/vo_postprocess/y416_to_r12l_fake.c#L341) |

## Dlouhé volby uv

Krátké volby a platformní aliasy jsou v [parseru](../../src/main.cpp). Zjištění dostupnosti za běhu začíná u `uv --list-modules`, `uv --capabilities` a u nápovědy podle třídy či modulu, např. `uv -x help` a `uv -x ultragrid_rtp:help`.

| Volba | Argument | Přepínač nebo identifikátor |
| --- | --- | --- |
| [`--audio-capture-channels`](../../src/main.cpp#L734) | required | `OPT_AUDIO_CAPTURE_CHANNELS` |
| [`--audio-capture-format`](../../src/main.cpp#L701) | required | `'a'` |
| [`--audio-channel-map`](../../src/main.cpp#L732) | required | `'U'` |
| [`--audio-codec`](../../src/main.cpp#L718) | required | `'A'` |
| [`--audio-delay`](../../src/main.cpp#L735) | required | `OPT_AUDIO_DELAY` |
| [`--audio-filter`](../../src/main.cpp#L708) | required | `'i'` |
| [`--audio-host`](../../src/main.cpp#L736) | required | `OPT_AUDIO_HOST` |
| [`--audio-protocol`](../../src/main.cpp#L737) | required | `OPT_AUDIO_PROTOCOL` |
| [`--audio-scale`](../../src/main.cpp#L738) | required | `OPT_AUDIO_SCALE` |
| [`--capabilities`](../../src/main.cpp#L702) | optional | `'b'` |
| [`--capture`](../../src/main.cpp#L710) | required | `'t'` |
| [`--capture-filter`](../../src/main.cpp#L722) | required | `'F'` |
| [`--client`](../../src/main.cpp#L719) | no | `'C'` |
| [`--compress`](../../src/main.cpp#L703) | required | `'c'` |
| [`--control-port`](../../src/main.cpp#L712) | required | `'n'` |
| [`--conv-policy`](../../src/main.cpp#L741) | required | `OPT_PIXFMT_CONV_POLICY` |
| [`--cuda-device`](../../src/main.cpp#L720) | required | `'D'` |
| [`--display`](../../src/main.cpp#L704) | required | `'d'` |
| [`--echo-cancellation`](../../src/main.cpp#L739) | no | `OPT_ECHO_CANCELLATION` |
| [`--encryption`](../../src/main.cpp#L705) | required | `'e'` |
| [`--fec`](../../src/main.cpp#L706) | required | `'f'` |
| [`--fullhelp`](../../src/main.cpp#L723) | no | `'H'` |
| [`--help`](../../src/main.cpp#L707) | no | `'h'` |
| [`--limit-bitrate`](../../src/main.cpp#L709) | required | `'l'` |
| [`--list-modules`](../../src/main.cpp#L725) | no | `'L'` |
| [`--mcast-if`](../../src/main.cpp#L740) | required | `OPT_MCAST_IF` |
| [`--mode`](../../src/main.cpp#L726) | required | `'M'` |
| [`--mtu`](../../src/main.cpp#L711) | required | `'m'` |
| [`--nat-traverse`](../../src/main.cpp#L727) | optional | `'N'` |
| [`--param`](../../src/main.cpp#L728) | required | `'O'` |
| [`--pix-fmts`](../../src/main.cpp#L742) | no | `OPT_PIX_FMTS` |
| [`--playback`](../../src/main.cpp#L724) | required | `'I'` |
| [`--port`](../../src/main.cpp#L729) | required | `'P'` |
| [`--postprocess`](../../src/main.cpp#L713) | required | `'p'` |
| [`--protocol`](../../src/main.cpp#L717) | required | `'x'` |
| [`--receive`](../../src/main.cpp#L714) | required | `'r'` |
| [`--record`](../../src/main.cpp#L721) | optional | `'E'` |
| [`--rtsp-server`](../../src/main.cpp#L743) | optional | `OPT_RTSP_SERVER` |
| [`--send`](../../src/main.cpp#L715) | required | `'s'` |
| [`--server`](../../src/main.cpp#L730) | no | `'S'` |
| [`--ttl`](../../src/main.cpp#L731) | required | `'T'` |
| [`--verbose`](../../src/main.cpp#L733) | optional | `'V'` |
| [`--version`](../../src/main.cpp#L716) | no | `'v'` |
| [`--video-codecs`](../../src/main.cpp#L744) | no | `OPT_VIDEO_CODECS` |
| [`--video-protocol`](../../src/main.cpp#L745) | required | `OPT_VIDEO_PROTOCOL` |
| [`--window-title`](../../src/main.cpp#L746) | required | `OPT_WINDOW_TITLE` |

## Rozšířené parametry uv

- `aja-fourcc` · [src/video_capture/aja.cpp:301](../../src/video_capture/aja.cpp#L301)
- `allow-unknown-params` · [src/host.cpp:1468](../../src/host.cpp#L1468)
- `alsa-play-period-size` · [src/audio/playback/alsa.c:499](../../src/audio/playback/alsa.c#L499)
- `alsa-playback-api` · [src/audio/playback/alsa.c:847](../../src/audio/playback/alsa.c#L847)
- `alsa-playback-buffer` · [src/audio/playback/alsa.c:453](../../src/audio/playback/alsa.c#L453)
- `audio-buffer-len` · [src/host.cpp:1470](../../src/host.cpp#L1470)
- `audio-cap-frames` · [src/host.cpp:1472](../../src/host.cpp#L1472)
- `audio-dec-format` · [src/audio/audio.cpp:473](../../src/audio/audio.cpp#L473)
- `audio-disable-adaptive-buffer` · [src/host.cpp:1474](../../src/host.cpp#L1474)
- `audio-lavc-decoder` · [src/audio/codec/libavcodec.c:222](../../src/audio/codec/libavcodec.c#L222)
- `audio-lavc-encoder` · [src/audio/codec/libavcodec.c:224](../../src/audio/codec/libavcodec.c#L224)
- `audioenc-frame-duration` · [src/audio/codec/libavcodec.c:217](../../src/audio/codec/libavcodec.c#L217)
- `ca-disable-adaptive-buf` · [src/audio/playback/coreaudio.c:153](../../src/audio/playback/coreaudio.c#L153)
- `color` · [src/host.cpp:1476](../../src/host.cpp#L1476)
- `color-601` · [src/color_space.c:133](../../src/color_space.c#L133)
- `control-accept-global` · [src/control_socket.c:789](../../src/control_socket.c#L789)
- `control-report-audio-ch-count` · [src/control_socket.c:175](../../src/control_socket.c#L175)
- `debug-dump` · [src/debug.cpp:320](../../src/debug.cpp#L320)
- `decoder-drop-policy` · [src/rtp/video_decoders.cpp:616](../../src/rtp/video_decoders.cpp#L616)
- `decoder-use-codec` · [src/rtp/video_decoders.cpp:847](../../src/rtp/video_decoders.cpp#L847)
- `disable-keyboard-control` · [src/keyboard_control.cpp:233](../../src/keyboard_control.cpp#L233)
- `echo-cancel-delay` · [src/audio/echo.cpp:123](../../src/audio/echo.cpp#L123)
- `echo-cancel-dump-audio` · [src/audio/echo.cpp:91](../../src/audio/echo.cpp#L91)
- `echo-cancel-filter-length` · [src/audio/echo.cpp:119](../../src/audio/echo.cpp#L119)
- `errors-fatal` · [src/host.cpp:1215](../../src/host.cpp#L1215)
- `force-lavd-decoder` · [src/video_decompress/libavcodec.c:342](../../src/video_decompress/libavcodec.c#L342)
- `j2k-dec-cpu-thread-count` · [src/video_decompress/cmpto_j2k.cpp:308](../../src/video_decompress/cmpto_j2k.cpp#L308)
- `j2k-dec-encoder-queue` · [src/video_decompress/cmpto_j2k.cpp:317](../../src/video_decompress/cmpto_j2k.cpp#L317)
- `j2k-dec-img-limit` · [src/video_decompress/cmpto_j2k.cpp:310](../../src/video_decompress/cmpto_j2k.cpp#L310)
- `j2k-dec-mem-limit` · [src/video_decompress/cmpto_j2k.cpp:301](../../src/video_decompress/cmpto_j2k.cpp#L301)
- `j2k-dec-queue-len` · [src/video_decompress/cmpto_j2k.cpp:315](../../src/video_decompress/cmpto_j2k.cpp#L315)
- `j2k-dec-tile-limit` · [src/video_decompress/cmpto_j2k.cpp:303](../../src/video_decompress/cmpto_j2k.cpp#L303)
- `j2k-dec-use-cpu` · [src/video_decompress/cmpto_j2k.cpp:306](../../src/video_decompress/cmpto_j2k.cpp#L306)
- `j2k-dec-use-cuda` · [src/video_decompress/cmpto_j2k.cpp:299](../../src/video_decompress/cmpto_j2k.cpp#L299)
- `keep-pixfmt` · [src/video_compress/libavcodec.cpp:725](../../src/video_compress/libavcodec.cpp#L725)
- `lavc-log-level` · [src/libavcodec/lavc_common.c:190](../../src/libavcodec/lavc_common.c#L190)
- `lavc-rc-buffer-size-factor` · [src/video_compress/libavcodec.cpp:1984](../../src/video_compress/libavcodec.cpp#L1984)
- `lavc-use-codec` · [src/video_compress/libavcodec.cpp:1023](../../src/video_compress/libavcodec.cpp#L1023)
- `lavd-accept-corrupted` · [src/video_decompress/libavcodec.c:1136](../../src/video_decompress/libavcodec.c#L1136)
- `lavd-thread-count` · [src/video_decompress/libavcodec.c:147](../../src/video_decompress/libavcodec.c#L147)
- `ldgm-device` · [src/rtp/ldgm.cpp:211](../../src/rtp/ldgm.cpp#L211)
- `log-color` · [src/utils/color_out.c:78](../../src/utils/color_out.c#L78)
- `log-nocolor` · [src/utils/color_out.c:80](../../src/utils/color_out.c#L80)
- `low-latency-audio` · [src/host.cpp:1478](../../src/host.cpp#L1478)
- `resampler` · [src/audio/resampler.cpp:357](../../src/audio/resampler.cpp#L357)
- `soft-resample` · [src/audio/postprocess.c:154](../../src/audio/postprocess.c#L154)
- `stderr-buf` · [src/host.cpp:261](../../src/host.cpp#L261)
- `stdout-buf` · [src/host.cpp:258](../../src/host.cpp#L258)
- `udp-disable-multi-socket` · [src/rtp/net_udp.c:1024](../../src/rtp/net_udp.c#L1024)
- `udp-queue-len` · [src/rtp/net_udp.c:1020](../../src/rtp/net_udp.c#L1020)
- `use-hw-accel` · [src/video_decompress/libavcodec.c:346](../../src/video_decompress/libavcodec.c#L346)
- `window-title` · [src/host.cpp:1481](../../src/host.cpp#L1481)

## Volby sestavení

Zde je zapsána forma `--enable-…` či `--with-…`. Výchozí hodnoty, protějšky `--disable-…` a `--without-…` a skutečné podmínky viz příslušná deklarace.

- [`--enable-aes67_play`](../../configure.ac#L3046)
- [`--enable-aja`](../../configure.ac#L1056)
- [`--enable-all`](../../configure.ac#L207)
- [`--enable-alsa`](../../configure.ac#L3072)
- [`--enable-avfoundation`](../../configure.ac#L1385)
- [`--enable-bitflow`](../../configure.ac#L3481)
- [`--enable-blank`](../../configure.ac#L1848)
- [`--enable-bluefish444`](../../configure.ac#L988)
- [`--enable-caca`](../../configure.ac#L1598)
- [`--enable-cineform`](../../configure.ac#L3598)
- [`--enable-cmpto-j2k`](../../configure.ac#L3500)
- [`--enable-coreaudio`](../../configure.ac#L3100)
- [`--enable-cuda`](../../configure.ac#L565)
- [`--enable-cuda-dxt`](../../configure.ac#L2705)
- [`--enable-debug`](../../configure.ac#L465)
- [`--enable-decklink`](../../configure.ac#L900)
- [`--enable-deltacast`](../../configure.ac#L1197)
- [`--enable-drm_disp`](../../configure.ac#L2168)
- [`--enable-dshow`](../../configure.ac#L2249)
- [`--enable-dvs`](../../configure.ac#L823)
- [`--enable-file`](../../configure.ac#L2119)
- [`--enable-fluidsynth`](../../configure.ac#L3748)
- [`--enable-gl`](../../configure.ac#L726)
- [`--enable-gl-display`](../../configure.ac#L2196)
- [`--enable-gpujpeg`](../../configure.ac#L2642)
- [`--enable-gpujpeg_to_dxt`](../../configure.ac#L2729)
- [`--enable-gpustitch`](../../configure.ac#L2753)
- [`--enable-holepunch`](../../configure.ac#L1142)
- [`--enable-ihdtv`](../../configure.ac#L3274)
- [`--enable-ipv6`](../../configure.ac#L473)
- [`--enable-jack`](../../configure.ac#L3008)
- [`--enable-jack-transport`](../../configure.ac#L3001)
- [`--enable-jpegxs`](../../configure.ac#L2554)
- [`--enable-lavc-cuda-conv`](../../configure.ac#L2039)
- [`--enable-lavc-hw-accel-vaapi`](../../configure.ac#L1954)
- [`--enable-lavc-hw-accel-vdpau`](../../configure.ac#L1947)
- [`--enable-ldgm`](../../configure.ac#L3360)
- [`--enable-ldgm-gpu`](../../configure.ac#L3375)
- [`--enable-libavcodec`](../../configure.ac#L2032)
- [`--enable-libbacktrace`](../../configure.ac#L521)
- [`--enable-libswscale`](../../configure.ac#L1993)
- [`--enable-man`](../../configure.ac#L339)
- [`--enable-mpegts`](../../configure.ac#L1794)
- [`--enable-natpmp`](../../configure.ac#L3697)
- [`--enable-ndi`](../../configure.ac#L3552)
- [`--enable-object`](../../configure.ac#L3788)
- [`--enable-omt`](../../configure.ac#L3670)
- [`--enable-openapv`](../../configure.ac#L2586)
- [`--enable-opencv`](../../configure.ac#L1621)
- [`--enable-openssl`](../../configure.ac#L3292)
- [`--enable-panogl_disp`](../../configure.ac#L1542)
- [`--enable-pcp`](../../configure.ac#L3723)
- [`--enable-pipewire`](../../configure.ac#L2270)
- [`--enable-pipewire-audio`](../../configure.ac#L2301)
- [`--enable-pipewire-video`](../../configure.ac#L2326)
- [`--enable-plugins`](../../configure.ac#L396)
- [`--enable-portaudio`](../../configure.ac#L2856)
- [`--enable-profile`](../../configure.ac#L452)
- [`--enable-pyrowave`](../../configure.ac#L2614)
- [`--enable-qt`](../../configure.ac#L3189)
- [`--enable-reflector`](../../configure.ac#L3772)
- [`--enable-resize`](../../configure.ac#L1823)
- [`--enable-rt`](../../configure.ac#L427)
- [`--enable-rtdxt`](../../configure.ac#L2490)
- [`--enable-rtsp`](../../configure.ac#L1690)
- [`--enable-rtsp_server`](../../configure.ac#L1722)
- [`--enable-sage`](../../configure.ac#L2796)
- [`--enable-sage-native-dxt5ycocg`](../../configure.ac#L2802)
- [`--enable-scale`](../../configure.ac#L3127)
- [`--enable-screen`](../../configure.ac#L2358)
- [`--enable-sdl`](../../configure.ac#L1409)
- [`--enable-sdp-http`](../../configure.ac#L1771)
- [`--enable-soxr`](../../configure.ac#L2914)
- [`--enable-speexdsp`](../../configure.ac#L2891)
- [`--enable-spout`](../../configure.ac#L3426)
- [`--enable-static-qt`](../../configure.ac#L3196)
- [`--enable-swmix`](../../configure.ac#L2226)
- [`--enable-syphon`](../../configure.ac#L3403)
- [`--enable-testcard2`](../../configure.ac#L1880)
- [`--enable-text`](../../configure.ac#L3152)
- [`--enable-tracy`](../../configure.ac#L1165)
- [`--enable-uyvy`](../../configure.ac#L2525)
- [`--enable-v4l2`](../../configure.ac#L3226)
- [`--enable-video-mixer`](../../configure.ac#L3462)
- [`--enable-vulkan`](../../configure.ac#L1476)
- [`--enable-wasapi`](../../configure.ac#L3258)
- [`--enable-ximea`](../../configure.ac#L1299)
- [`--enable-ximea-runtime-linking`](../../configure.ac#L1306)
- [`--enable-xrgl_disp`](../../configure.ac#L1572)
- [`--enable-zfec`](../../configure.ac#L2938)
- [`--with-aja`](../../configure.ac#L1082)
- [`--with-bluefish444`](../../configure.ac#L997)
- [`--with-cineform`](../../configure.ac#L3609)
- [`--with-cuda`](../../configure.ac#L570)
- [`--with-cuda-compiler`](../../configure.ac#L651)
- [`--with-cuda-host-compiler`](../../configure.ac#L672)
- [`--with-deltacast`](../../configure.ac#L1203)
- [`--with-dvs`](../../configure.ac#L849)
- [`--with-live555`](../../configure.ac#L1729)
- [`--with-object-remove`](../../configure.ac#L3894)
- [`--with-sage`](../../configure.ac#L2807)
- [`--with-zfec`](../../configure.ac#L2942)

## Rozsah stromu

- `.github` · 57
- `.gitignore` · 1
- `.gitmodules` · 1
- `CONTRIBUTING.md` · 1
- `COPYRIGHT` · 1
- `Doxyfile` · 1
- `INSTALL` · 1
- `Makefile.in` · 1
- `NEWS` · 1
- `README.md` · 1
- `autogen.sh` · 1
- `configure.ac` · 1
- `cuda_dxt` · 6
- `data` · 39
- `doc` · 4
- `dxt_compress` · 25
- `ext-deps` · 26
- `gui` · 68
- `hd-rum-multi` · 5
- `ldgm` · 24
- `nat-helper` · 12
- `package_specs` · 172
- `share` · 8
- `src` · 105
- `src/audio` · 71
- `src/capture_filter` · 25
- `src/compat` · 20
- `src/crypto` · 10
- `src/cuda_wrapper` · 3
- `src/hd-rum-translator` · 5
- `src/ihdtv` · 2
- `src/jpegxs` · 2
- `src/libavcodec` · 14
- `src/openapv` · 4
- `src/rtp` · 29
- `src/rtsp` · 5
- `src/rxtx` · 12
- `src/utils` · 93
- `src/video_capture` · 34
- `src/video_compress` · 11
- `src/video_decompress` · 10
- `src/video_display` · 62
- `src/vo_postprocess` · 15
- `test` · 23
- `tools` · 19

## Wiki · 102 textových položek

Index zahrnuje i navigaci a archivní poznámky. Vydání a historický hardware posuzovat podle obsahu konkrétní stránky.

- [4K-Video-Settings](https://github.com/CESNET/UltraGrid/wiki/4K-Video-Settings)
- [AJA-HD10A](https://github.com/CESNET/UltraGrid/wiki/AJA-HD10A)
- [AJA-HDP](https://github.com/CESNET/UltraGrid/wiki/AJA-HDP)
- [AJA-Setup](https://github.com/CESNET/UltraGrid/wiki/AJA-Setup)
- [AJA](https://github.com/CESNET/UltraGrid/wiki/AJA)
- [Audio-Settings](https://github.com/CESNET/UltraGrid/wiki/Audio-Settings)
- [Audio-filters](https://github.com/CESNET/UltraGrid/wiki/Audio-filters)
- [Authors-and-Publications](https://github.com/CESNET/UltraGrid/wiki/Authors-and-Publications)
- [Available-additional-hardware](https://github.com/CESNET/UltraGrid/wiki/Available-additional-hardware)
- [Bluefish444-Setup](https://github.com/CESNET/UltraGrid/wiki/Bluefish444-Setup)
- [Build-FFmpeg](https://github.com/CESNET/UltraGrid/wiki/Build-FFmpeg)
- [Capabilities-output-format](https://github.com/CESNET/UltraGrid/wiki/Capabilities-output-format)
- [Capture-filters](https://github.com/CESNET/UltraGrid/wiki/Capture-filters)
- [Cards](https://github.com/CESNET/UltraGrid/wiki/Cards)
- [Centaurus-Setup-(Linux)](https://github.com/CESNET/UltraGrid/wiki/Centaurus-Setup-%28Linux%29)
- [Compile-UltraGrid-(Source)](https://github.com/CESNET/UltraGrid/wiki/Compile-UltraGrid-%28Source%29)
- [Compile-UltraGrid-(Windows)](https://github.com/CESNET/UltraGrid/wiki/Compile-UltraGrid-%28Windows%29)
- [Compression-Settings](https://github.com/CESNET/UltraGrid/wiki/Compression-Settings)
- [Control-port-API](https://github.com/CESNET/UltraGrid/wiki/Control-port-API)
- [Create-Application-Bundle](https://github.com/CESNET/UltraGrid/wiki/Create-Application-Bundle)
- [DELTACAST-DKMS](https://github.com/CESNET/UltraGrid/wiki/DELTACAST-DKMS)
- [DELTACAST-Setup-(Linux)](https://github.com/CESNET/UltraGrid/wiki/DELTACAST-Setup-%28Linux%29)
- [DELTACAST-Setup](https://github.com/CESNET/UltraGrid/wiki/DELTACAST-Setup)
- [DMA-Throughput-(Myricom)](https://github.com/CESNET/UltraGrid/wiki/DMA-Throughput-%28Myricom%29)
- [DVS-Centaurus](https://github.com/CESNET/UltraGrid/wiki/DVS-Centaurus)
- [DVS-HDStationOEM](https://github.com/CESNET/UltraGrid/wiki/DVS-HDStationOEM)
- [DVS](https://github.com/CESNET/UltraGrid/wiki/DVS)
- [DeckLink-IP](https://github.com/CESNET/UltraGrid/wiki/DeckLink-IP)
- [DeckLink-Setup](https://github.com/CESNET/UltraGrid/wiki/DeckLink-Setup)
- [Development](https://github.com/CESNET/UltraGrid/wiki/Development)
- [Device-Settings](https://github.com/CESNET/UltraGrid/wiki/Device-Settings)
- [Display-(SDL-or-GL)](https://github.com/CESNET/UltraGrid/wiki/Display-%28SDL-or-GL%29)
- [Download-UltraGrid](https://github.com/CESNET/UltraGrid/wiki/Download-UltraGrid)
- [Encryption](https://github.com/CESNET/UltraGrid/wiki/Encryption)
- [Extending-Network-Buffers](https://github.com/CESNET/UltraGrid/wiki/Extending-Network-Buffers)
- [FEC-Settings](https://github.com/CESNET/UltraGrid/wiki/FEC-Settings)
- [FastDXT-Setup-(Linux)](https://github.com/CESNET/UltraGrid/wiki/FastDXT-Setup-%28Linux%29)
- [H.264-error-resiliency](https://github.com/CESNET/UltraGrid/wiki/H.264-error-resiliency)
- [H.264-testing](https://github.com/CESNET/UltraGrid/wiki/H.264-testing)
- [HD-bandwidth](https://github.com/CESNET/UltraGrid/wiki/HD-bandwidth)
- [HD-card-latencies](https://github.com/CESNET/UltraGrid/wiki/HD-card-latencies)
- [Home](https://github.com/CESNET/UltraGrid/wiki/Home)
- [Hw.-acceleration-support](https://github.com/CESNET/UltraGrid/wiki/Hw.-acceleration-support)
- [IHDTV-Settings](https://github.com/CESNET/UltraGrid/wiki/IHDTV-Settings)
- [IPv6](https://github.com/CESNET/UltraGrid/wiki/IPv6)
- [Install-UltraGrid](https://github.com/CESNET/UltraGrid/wiki/Install-UltraGrid)
- [Intel-10GE-LR-cards](https://github.com/CESNET/UltraGrid/wiki/Intel-10GE-LR-cards)
- [Interlaced-Input](https://github.com/CESNET/UltraGrid/wiki/Interlaced-Input)
- [Jumbo-Frames-(Linux)](https://github.com/CESNET/UltraGrid/wiki/Jumbo-Frames-%28Linux%29)
- [Libavcodec-Compression](https://github.com/CESNET/UltraGrid/wiki/Libavcodec-Compression)
- [Live-web-streaming-with-Nginx](https://github.com/CESNET/UltraGrid/wiki/Live-web-streaming-with-Nginx)
- [Multipoint-Setup](https://github.com/CESNET/UltraGrid/wiki/Multipoint-Setup)
- [Myricom-Settings](https://github.com/CESNET/UltraGrid/wiki/Myricom-Settings)
- [NAT-traversal](https://github.com/CESNET/UltraGrid/wiki/NAT-traversal)
- [NDI](https://github.com/CESNET/UltraGrid/wiki/NDI)
- [Network-(Linux)](https://github.com/CESNET/UltraGrid/wiki/Network-%28Linux%29)
- [OS-Setup-UltraGrid](https://github.com/CESNET/UltraGrid/wiki/OS-Setup-UltraGrid)
- [PCIE-Utilization-(Myricom)](https://github.com/CESNET/UltraGrid/wiki/PCIE-Utilization-%28Myricom%29)
- [Panoramatic-360-degree-video](https://github.com/CESNET/UltraGrid/wiki/Panoramatic-360-degree-video)
- [Performance](https://github.com/CESNET/UltraGrid/wiki/Performance)
- [Portaudio-Setup-(Linux)](https://github.com/CESNET/UltraGrid/wiki/Portaudio-Setup-%28Linux%29)
- [RTDXT-Setup](https://github.com/CESNET/UltraGrid/wiki/RTDXT-Setup)
- [RTSP-Server,-SDP](https://github.com/CESNET/UltraGrid/wiki/RTSP-Server%2C-SDP)
- [Raspberry-Pi-display](https://github.com/CESNET/UltraGrid/wiki/Raspberry-Pi-display)
- [Recording-and-Playback](https://github.com/CESNET/UltraGrid/wiki/Recording-and-Playback)
- [Reflector-settings](https://github.com/CESNET/UltraGrid/wiki/Reflector-settings)
- [Resolutions](https://github.com/CESNET/UltraGrid/wiki/Resolutions)
- [Running-UltraGrid-from-macOS-bunde](https://github.com/CESNET/UltraGrid/wiki/Running-UltraGrid-from-macOS-bunde)
- [Running-UltraGrid](https://github.com/CESNET/UltraGrid/wiki/Running-UltraGrid)
- [SRT-encapsulation](https://github.com/CESNET/UltraGrid/wiki/SRT-encapsulation)
- [SW-Video-Mix](https://github.com/CESNET/UltraGrid/wiki/SW-Video-Mix)
- [Screen-Capture](https://github.com/CESNET/UltraGrid/wiki/Screen-Capture)
- [Set-Jumbo-Frames-(Linux)](https://github.com/CESNET/UltraGrid/wiki/Set-Jumbo-Frames-%28Linux%29)
- [Set-Jumbo-Frames-(Windows)](https://github.com/CESNET/UltraGrid/wiki/Set-Jumbo-Frames-%28Windows%29)
- [Set-Jumbo-Frames-(macOS)](https://github.com/CESNET/UltraGrid/wiki/Set-Jumbo-Frames-%28macOS%29)
- [Spout-and-Syphon](https://github.com/CESNET/UltraGrid/wiki/Spout-and-Syphon)
- [Stereoscopic-3D-Video-Settings](https://github.com/CESNET/UltraGrid/wiki/Stereoscopic-3D-Video-Settings)
- [Streaming-to-Wowza-media-server](https://github.com/CESNET/UltraGrid/wiki/Streaming-to-Wowza-media-server)
- [Syphon,-Spout-and-NDI](https://github.com/CESNET/UltraGrid/wiki/Syphon%2C-Spout-and-NDI)
- [System-requirements](https://github.com/CESNET/UltraGrid/wiki/System-requirements)
- [Tested-HW-configurations](https://github.com/CESNET/UltraGrid/wiki/Tested-HW-configurations)
- [Tested-cards](https://github.com/CESNET/UltraGrid/wiki/Tested-cards)
- [Traffic-shaping](https://github.com/CESNET/UltraGrid/wiki/Traffic-shaping)
- [Transcoding-reflector](https://github.com/CESNET/UltraGrid/wiki/Transcoding-reflector)
- [UltraGrid-Compatibility](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-Compatibility)
- [UltraGrid-FAQ](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-FAQ)
- [UltraGrid-Internal-Notes](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-Internal-Notes)
- [UltraGrid-Modules-macOS](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-Modules-macOS)
- [UltraGrid-Network-Check](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-Network-Check)
- [UltraGrid-Preliminaries-(Linux)](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-Preliminaries-%28Linux%29)
- [UltraGrid-Preliminaries-(macOS)](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-Preliminaries-%28macOS%29)
- [UltraGrid-Setup-(Linux)](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-Setup-%28Linux%29)
- [UltraGrid-packet-types](https://github.com/CESNET/UltraGrid/wiki/UltraGrid-packet-types)
- [Use-Cases](https://github.com/CESNET/UltraGrid/wiki/Use-Cases)
- [Useful-Links](https://github.com/CESNET/UltraGrid/wiki/Useful-Links)
- [Video-Filters](https://github.com/CESNET/UltraGrid/wiki/Video-Filters)
- [Video-Switcher](https://github.com/CESNET/UltraGrid/wiki/Video-Switcher)
- [Videoconferencing-Mode](https://github.com/CESNET/UltraGrid/wiki/Videoconferencing-Mode)
- [Vsync-SDL-GL](https://github.com/CESNET/UltraGrid/wiki/Vsync-SDL-GL)
- [_Footer](https://github.com/CESNET/UltraGrid/wiki/_Footer)
- [_Sidebar](https://github.com/CESNET/UltraGrid/wiki/_Sidebar)
- [macOS-allow-unidentified-developer](https://github.com/CESNET/UltraGrid/wiki/macOS-allow-unidentified-developer)

## Přílohy wiki · 30 PDF

Manuály k hardwaru, paketové specifikace, měření, schémata a historické prezentace.

- [AJA_manual_HD10A_2ndSeries.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/AJA_manual_HD10A_2ndSeries.pdf)
- [AJA_manual_HDP.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/AJA_manual_HDP.pdf)
- [AJA_pathDelays.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/AJA_pathDelays.pdf)
- [Aux_pkt_fmts.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Aux_pkt_fmts.pdf)
- [BROWN-CANS2005-iGrid-01Nov2005_3A.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/BROWN-CANS2005-iGrid-01Nov2005_3A.pdf)
- [Bob_ii_ig_v1_0.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Bob_ii_ig_v1_0.pdf)
- [COS_3.NP.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/COS_3.NP.pdf)
- [Centaurus_ig_v1_0.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Centaurus_ig_v1_0.pdf)
- [Chelsio10GbE_MPI_report.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Chelsio10GbE_MPI_report.pdf)
- [Chelsio_10gbe_fujitsu.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Chelsio_10gbe_fujitsu.pdf)
- [DS16_harmonogram_v3.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/DS16_harmonogram_v3.pdf)
- [Decklink_4K_Extreme.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Decklink_4K_Extreme.pdf)
- [Evl.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Evl.pdf)
- [Flyer.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Flyer.pdf)
- [HD-scheme-v1.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/HD-scheme-v1.pdf)
- [HD-scheme-v2.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/HD-scheme-v2.pdf)
- [HDmulticonf.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/HDmulticonf.pdf)
- [HDmulticonf8.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/HDmulticonf8.pdf)
- [Main.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Main.pdf)
- [Opteron.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Opteron.pdf)
- [Pckt_fmts.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Pckt_fmts.pdf)
- [Perf-1rum-1GE.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Perf-1rum-1GE.pdf)
- [Perf-nrum-1GE.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Perf-nrum-1GE.pdf)
- [Presentation.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Presentation.pdf)
- [RATreport.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/RATreport.pdf)
- [Splitter-1.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Splitter-1.pdf)
- [Splitter-2.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Splitter-2.pdf)
- [Splitter-3.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Splitter-3.pdf)
- [StarLight-scheme-v1.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/StarLight-scheme-v1.pdf)
- [Xeon.pdf](https://raw.githubusercontent.com/wiki/CESNET/UltraGrid/Media/Xeon.pdf)
