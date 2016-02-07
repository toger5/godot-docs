.. _class_AudioServer:

AudioServer
===========

Inherits: :ref:`Object<class_object>`
-------------------------------------

Category: Core
--------------

Brief Description
-----------------

Server interface for low level audio access.

Member Functions
----------------

+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_rid>`            | :ref:`sample_create<class_AudioServer_sample_create>`  **(** :ref:`int<class_int>` format, :ref:`bool<class_bool>` stereo, :ref:`int<class_int>` length  **)**                                                                             |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`sample_set_description<class_AudioServer_sample_set_description>`  **(** :ref:`RID<class_rid>` sample, :ref:`String<class_string>` description  **)**                                                                                |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_string>`      | :ref:`sample_get_description<class_AudioServer_sample_get_description>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                   |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`sample_get_format<class_AudioServer_sample_get_format>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                             |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`          | :ref:`sample_is_stereo<class_AudioServer_sample_is_stereo>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                               |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`sample_get_length<class_AudioServer_sample_get_length>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                             |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`sample_set_signed_data<class_AudioServer_sample_set_signed_data>`  **(** :ref:`RID<class_rid>` sample, :ref:`RealArray<class_realarray>` data  **)**                                                                                 |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`sample_set_data<class_AudioServer_sample_set_data>`  **(** :ref:`RID<class_rid>` sample, :ref:`RawArray<class_rawarray>` data  **)**                                                                                                 |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`RawArray<class_rawarray>`  | :ref:`sample_get_data<class_AudioServer_sample_get_data>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                                 |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`sample_set_mix_rate<class_AudioServer_sample_set_mix_rate>`  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` mix_rate  **)**                                                                                               |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`sample_get_mix_rate<class_AudioServer_sample_get_mix_rate>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                         |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`sample_set_loop_format<class_AudioServer_sample_set_loop_format>`  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` loop_format  **)**                                                                                      |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`sample_get_loop_format<class_AudioServer_sample_get_loop_format>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                   |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`sample_set_loop_begin<class_AudioServer_sample_set_loop_begin>`  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` pos  **)**                                                                                                |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`sample_get_loop_begin<class_AudioServer_sample_get_loop_begin>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                     |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`sample_set_loop_end<class_AudioServer_sample_set_loop_end>`  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` pos  **)**                                                                                                    |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`sample_get_loop_end<class_AudioServer_sample_get_loop_end>`  **(** :ref:`RID<class_rid>` sample  **)** const                                                                                                                         |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`RID<class_rid>`            | :ref:`voice_create<class_AudioServer_voice_create>`  **(** **)**                                                                                                                                                                           |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_play<class_AudioServer_voice_play>`  **(** :ref:`RID<class_rid>` voice, :ref:`RID<class_rid>` sample  **)**                                                                                                                    |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_set_volume<class_AudioServer_voice_set_volume>`  **(** :ref:`RID<class_rid>` voice, :ref:`float<class_float>` volume  **)**                                                                                                    |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_set_pan<class_AudioServer_voice_set_pan>`  **(** :ref:`RID<class_rid>` voice, :ref:`float<class_float>` pan, :ref:`float<class_float>` depth=0, :ref:`float<class_float>` height=0  **)**                                      |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_set_filter<class_AudioServer_voice_set_filter>`  **(** :ref:`RID<class_rid>` voice, :ref:`int<class_int>` type, :ref:`float<class_float>` cutoff, :ref:`float<class_float>` resonance, :ref:`float<class_float>` gain=0  **)** |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_set_chorus<class_AudioServer_voice_set_chorus>`  **(** :ref:`RID<class_rid>` voice, :ref:`float<class_float>` chorus  **)**                                                                                                    |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_set_reverb<class_AudioServer_voice_set_reverb>`  **(** :ref:`RID<class_rid>` voice, :ref:`int<class_int>` room, :ref:`float<class_float>` reverb  **)**                                                                        |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_set_mix_rate<class_AudioServer_voice_set_mix_rate>`  **(** :ref:`RID<class_rid>` voice, :ref:`int<class_int>` rate  **)**                                                                                                      |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_set_positional<class_AudioServer_voice_set_positional>`  **(** :ref:`RID<class_rid>` voice, :ref:`bool<class_bool>` enabled  **)**                                                                                             |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_volume<class_AudioServer_voice_get_volume>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                                |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_pan<class_AudioServer_voice_get_pan>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                                      |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_pan_height<class_AudioServer_voice_get_pan_height>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                        |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_pan_depth<class_AudioServer_voice_get_pan_depth>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                          |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`voice_get_filter_type<class_AudioServer_voice_get_filter_type>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                      |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_filter_cutoff<class_AudioServer_voice_get_filter_cutoff>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                  |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_filter_resonance<class_AudioServer_voice_get_filter_resonance>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                            |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_chorus<class_AudioServer_voice_get_chorus>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                                |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`voice_get_reverb_type<class_AudioServer_voice_get_reverb_type>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                      |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`voice_get_reverb<class_AudioServer_voice_get_reverb>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                                |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`            | :ref:`voice_get_mix_rate<class_AudioServer_voice_get_mix_rate>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                            |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`          | :ref:`voice_is_positional<class_AudioServer_voice_is_positional>`  **(** :ref:`RID<class_rid>` voice  **)** const                                                                                                                          |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`voice_stop<class_AudioServer_voice_stop>`  **(** :ref:`RID<class_rid>` voice  **)**                                                                                                                                                  |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`free_rid<class_AudioServer_free_rid>`  **(** :ref:`RID<class_rid>` rid  **)**                                                                                                                                                        |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_stream_global_volume_scale<class_AudioServer_set_stream_global_volume_scale>`  **(** :ref:`float<class_float>` scale  **)**                                                                                                      |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`get_stream_global_volume_scale<class_AudioServer_get_stream_global_volume_scale>`  **(** **)** const                                                                                                                                 |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_fx_global_volume_scale<class_AudioServer_set_fx_global_volume_scale>`  **(** :ref:`float<class_float>` scale  **)**                                                                                                              |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`get_fx_global_volume_scale<class_AudioServer_get_fx_global_volume_scale>`  **(** **)** const                                                                                                                                         |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_event_voice_global_volume_scale<class_AudioServer_set_event_voice_global_volume_scale>`  **(** :ref:`float<class_float>` scale  **)**                                                                                            |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>`        | :ref:`get_event_voice_global_volume_scale<class_AudioServer_get_event_voice_global_volume_scale>`  **(** **)** const                                                                                                                       |
+----------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Numeric Constants
-----------------

- **SAMPLE_FORMAT_PCM8** = **0** --- Sample format is 8 bits, signed.
- **SAMPLE_FORMAT_PCM16** = **1** --- Sample format is 16 bits, little-endian, signed.
- **SAMPLE_FORMAT_IMA_ADPCM** = **2** --- Sample format is IMA-ADPCM compressed.
- **SAMPLE_LOOP_NONE** = **0** --- Sample does not loop.
- **SAMPLE_LOOP_FORWARD** = **1** --- Sample loops in forward mode.
- **SAMPLE_LOOP_PING_PONG** = **2** --- Sample loops in a bidirectional way.
- **FILTER_NONE** = **0** --- Filter is disabled.
- **FILTER_LOWPASS** = **1** --- Filter is a resonant lowpass.
- **FILTER_BANDPASS** = **2** --- Filter is a resonant bandpass.
- **FILTER_HIPASS** = **3** --- Filter is a resonant highpass.
- **FILTER_NOTCH** = **4** --- Filter is a notch (band reject).
- **FILTER_BANDLIMIT** = **6** --- Filter is a bandlimit (resonance used as highpass).
- **REVERB_SMALL** = **0** --- Small reverb room (closet, bathroom, etc).
- **REVERB_MEDIUM** = **1** --- Medium reverb room (living room)
- **REVERB_LARGE** = **2** --- Large reverb room (warehouse).
- **REVERB_HALL** = **3** --- Large reverb room with long decay.

Description
-----------

AudioServer is a low level server interface for audio access. It is in charge of creating sample data (playable audio) as well as its playback via a voice interface.

Member Function Description
---------------------------

.. _class_AudioServer_sample_create:

- :ref:`RID<class_rid>`  **sample_create**  **(** :ref:`int<class_int>` format, :ref:`bool<class_bool>` stereo, :ref:`int<class_int>` length  **)**

Create an audio sample, return a :ref:`RID<class_rid>` referencing it. The sample will be created with a given format (from the SAMPLE_FORMAT_* enum), a total length (in samples, not bytes), in either stereo or mono.

Even if a stereo sample consists of a left sample and a right sample, it still counts as one sample for length purposes.

.. _class_AudioServer_sample_set_description:

- void  **sample_set_description**  **(** :ref:`RID<class_rid>` sample, :ref:`String<class_string>` description  **)**

Set the description of an audio sample. Mainly used for organization.

.. _class_AudioServer_sample_get_description:

- :ref:`String<class_string>`  **sample_get_description**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the description of an audio sample. Mainly used for organization.

.. _class_AudioServer_sample_get_format:

- :ref:`int<class_int>`  **sample_get_format**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the format of the audio sample, in the form of the SAMPLE_FORMAT_* enum.

.. _class_AudioServer_sample_is_stereo:

- :ref:`bool<class_bool>`  **sample_is_stereo**  **(** :ref:`RID<class_rid>` sample  **)** const

Return whether the sample is stereo (2 channels).

.. _class_AudioServer_sample_get_length:

- :ref:`int<class_int>`  **sample_get_length**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the length in samples (not bytes) of the audio sample. Even if a stereo sample consists of a left sample and a right sample, it still counts as one sample for length purposes.

.. _class_AudioServer_sample_set_signed_data:

- void  **sample_set_signed_data**  **(** :ref:`RID<class_rid>` sample, :ref:`RealArray<class_realarray>` data  **)**

Set the sample data for a given sample as an array of floats. The length must be equal to the sample lenght or an error will be produced.

For this method, a stereo sample is made from two samples. Thus, in case of a stereo sample, the array length must be twice the length returned by :ref:`sample_get_length<AudioServer_sample_get_length>`.

Trying to alter a SAMPLE_FORMAT_IMA_ADPCM sample is not supported. It will throw an error to the console, but will not alter the sample data.

.. _class_AudioServer_sample_set_data:

- void  **sample_set_data**  **(** :ref:`RID<class_rid>` sample, :ref:`RawArray<class_rawarray>` data  **)**

Set the sample data for a given sample as an array of bytes. The length must be equal to the sample lenght expected in bytes or an error will be produced. The byte length can be calculated as follows:

Get the sample length (:ref:`get_sample_length<AudioServer_get_sample_length>`).

If the sample format is SAMPLE_FORMAT_PCM16, multiply it by 2.

If the sample format is SAMPLE_FORMAT_IMA_ADPCM, divide it by 2 (rounding any fraction up), then add 4.

If the sample is stereo (:ref:`sample_is_stereo<AudioServer_sample_is_stereo>`), multiply it by 2.

.. _class_AudioServer_sample_get_data:

- :ref:`RawArray<class_rawarray>`  **sample_get_data**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the sample data as an array of bytes. The length will be the expected length in bytes.

.. _class_AudioServer_sample_set_mix_rate:

- void  **sample_set_mix_rate**  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` mix_rate  **)**

Change the default mix rate of a given sample.

.. _class_AudioServer_sample_get_mix_rate:

- :ref:`int<class_int>`  **sample_get_mix_rate**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the mix rate of the given sample.

.. _class_AudioServer_sample_set_loop_format:

- void  **sample_set_loop_format**  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` loop_format  **)**

Set the loop format for a sample from the SAMPLE_LOOP_* enum. As a warning, Ping Pong loops may not be available on some hardware-mixing platforms.

.. _class_AudioServer_sample_get_loop_format:

- :ref:`int<class_int>`  **sample_get_loop_format**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the loop format for a sample, as a value from the SAMPLE_LOOP_* enum.

.. _class_AudioServer_sample_set_loop_begin:

- void  **sample_set_loop_begin**  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` pos  **)**

Set the initial loop point of a sample. Only has effect if sample loop is enabled. See :ref:`sample_set_loop_format<AudioServer_sample_set_loop_format>`.

.. _class_AudioServer_sample_get_loop_begin:

- :ref:`int<class_int>`  **sample_get_loop_begin**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the initial loop point of a sample. Only has effect if sample loop is enabled. See :ref:`sample_set_loop_format<AudioServer_sample_set_loop_format>`.

.. _class_AudioServer_sample_set_loop_end:

- void  **sample_set_loop_end**  **(** :ref:`RID<class_rid>` sample, :ref:`int<class_int>` pos  **)**

Set the final loop point of a sample. Only has effect if sample loop is enabled. See :ref:`sample_set_loop_format<AudioServer_sample_set_loop_format>`.

.. _class_AudioServer_sample_get_loop_end:

- :ref:`int<class_int>`  **sample_get_loop_end**  **(** :ref:`RID<class_rid>` sample  **)** const

Return the final loop point of a sample. Only has effect if sample loop is enabled. See :ref:`sample_set_loop_format<AudioServer_sample_set_loop_format>`.

.. _class_AudioServer_voice_create:

- :ref:`RID<class_rid>`  **voice_create**  **(** **)**

Allocate a voice for playback. Voices are persistent. A voice can play a single sample at the same time. See :ref:`sample_create<AudioServer_sample_create>`.

.. _class_AudioServer_voice_play:

- void  **voice_play**  **(** :ref:`RID<class_rid>` voice, :ref:`RID<class_rid>` sample  **)**

Start playback of a given voice using a given sample. If the voice was already playing it will be restarted.

.. _class_AudioServer_voice_set_volume:

- void  **voice_set_volume**  **(** :ref:`RID<class_rid>` voice, :ref:`float<class_float>` volume  **)**

Change the volume of a currently playing voice. Volume is expressed as linear gain where 0.0 is mute and 1.0 is default.

.. _class_AudioServer_voice_set_pan:

- void  **voice_set_pan**  **(** :ref:`RID<class_rid>` voice, :ref:`float<class_float>` pan, :ref:`float<class_float>` depth=0, :ref:`float<class_float>` height=0  **)**

Change the pan of a currently playing voice and, optionally, the depth and height for a positional/3D sound. Panning values are expressed within the -1 to +1 range.

.. _class_AudioServer_voice_set_filter:

- void  **voice_set_filter**  **(** :ref:`RID<class_rid>` voice, :ref:`int<class_int>` type, :ref:`float<class_float>` cutoff, :ref:`float<class_float>` resonance, :ref:`float<class_float>` gain=0  **)**

Set a resonant filter post processing for the voice. Filter type is a value from the FILTER_* enum.

.. _class_AudioServer_voice_set_chorus:

- void  **voice_set_chorus**  **(** :ref:`RID<class_rid>` voice, :ref:`float<class_float>` chorus  **)**

Set chorus send post processing for the voice (from 0 to 1).

.. _class_AudioServer_voice_set_reverb:

- void  **voice_set_reverb**  **(** :ref:`RID<class_rid>` voice, :ref:`int<class_int>` room, :ref:`float<class_float>` reverb  **)**

Set the reverb send post processing for the voice (from 0 to 1) and the reverb type, from the REVERB_* enum.

.. _class_AudioServer_voice_set_mix_rate:

- void  **voice_set_mix_rate**  **(** :ref:`RID<class_rid>` voice, :ref:`int<class_int>` rate  **)**

Set a different playback mix rate for the given voice.

.. _class_AudioServer_voice_set_positional:

- void  **voice_set_positional**  **(** :ref:`RID<class_rid>` voice, :ref:`bool<class_bool>` enabled  **)**

Set wether a given voice is positional. This is only interpreted as a hint and used for backends that may support binaural encoding.

.. _class_AudioServer_voice_get_volume:

- :ref:`float<class_float>`  **voice_get_volume**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current volume for a given voice.

.. _class_AudioServer_voice_get_pan:

- :ref:`float<class_float>`  **voice_get_pan**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current pan for a given voice (-1 to +1 range).

.. _class_AudioServer_voice_get_pan_height:

- :ref:`float<class_float>`  **voice_get_pan_height**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current pan height for a given voice (-1 to +1 range).

.. _class_AudioServer_voice_get_pan_depth:

- :ref:`float<class_float>`  **voice_get_pan_depth**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current pan depth for a given voice (-1 to +1 range).

.. _class_AudioServer_voice_get_filter_type:

- :ref:`int<class_int>`  **voice_get_filter_type**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current selected filter type for a given voice, from the FILTER_* enum.

.. _class_AudioServer_voice_get_filter_cutoff:

- :ref:`float<class_float>`  **voice_get_filter_cutoff**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current filter cutoff (in hz) for a given voice.

.. _class_AudioServer_voice_get_filter_resonance:

- :ref:`float<class_float>`  **voice_get_filter_resonance**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current filter resonance for a given voice.

.. _class_AudioServer_voice_get_chorus:

- :ref:`float<class_float>`  **voice_get_chorus**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current chorus send for a given voice (0 to 1).

.. _class_AudioServer_voice_get_reverb_type:

- :ref:`int<class_int>`  **voice_get_reverb_type**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current reverb type for a given voice from the REVERB_* enum.

.. _class_AudioServer_voice_get_reverb:

- :ref:`float<class_float>`  **voice_get_reverb**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current reverb send for a given voice (0 to 1).

.. _class_AudioServer_voice_get_mix_rate:

- :ref:`int<class_int>`  **voice_get_mix_rate**  **(** :ref:`RID<class_rid>` voice  **)** const

Return the current mix rate for a given voice.

.. _class_AudioServer_voice_is_positional:

- :ref:`bool<class_bool>`  **voice_is_positional**  **(** :ref:`RID<class_rid>` voice  **)** const

Return wether the current voice is positional. See :ref:`voice_set_positional<AudioServer_voice_set_positional>`.

.. _class_AudioServer_voice_stop:

- void  **voice_stop**  **(** :ref:`RID<class_rid>` voice  **)**

Stop a given voice.

.. _class_AudioServer_free_rid:

- void  **free_rid**  **(** :ref:`RID<class_rid>` rid  **)**

Free a :ref:`RID<class_rid>` resource.

.. _class_AudioServer_set_stream_global_volume_scale:

- void  **set_stream_global_volume_scale**  **(** :ref:`float<class_float>` scale  **)**

Set global scale for stream playback. Default is 1.0.

.. _class_AudioServer_get_stream_global_volume_scale:

- :ref:`float<class_float>`  **get_stream_global_volume_scale**  **(** **)** const

Return the global scale for stream playback.

.. _class_AudioServer_set_fx_global_volume_scale:

- void  **set_fx_global_volume_scale**  **(** :ref:`float<class_float>` scale  **)**

Set global scale for all voices (not including streams). Default is 1.0.

.. _class_AudioServer_get_fx_global_volume_scale:

- :ref:`float<class_float>`  **get_fx_global_volume_scale**  **(** **)** const

Return the global scale for all voices.

.. _class_AudioServer_set_event_voice_global_volume_scale:

- void  **set_event_voice_global_volume_scale**  **(** :ref:`float<class_float>` scale  **)**

Set global scale for event-based stream (:ref:`EventStream<class_eventstream>`) playback. Default is 1.0.

.. _class_AudioServer_get_event_voice_global_volume_scale:

- :ref:`float<class_float>`  **get_event_voice_global_volume_scale**  **(** **)** const

Return the global scale for event-based stream playback.

